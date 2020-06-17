---
title: Microsoft Graph 更改日志
description: 此更改日志涵盖了 Microsoft Graph 变更，包括 v1.0 和 beta 终结点 Microsoft Graph API。
author: MSGraphDocsVteam
localization_priority: Priority
ms.openlocfilehash: 4b50621b9472bf7e60be6af4a901c5d888343cd8
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744076"
---
# <a name="changelog-for-microsoft-graph"></a>Microsoft Graph 更改日志

此变更日志涵盖 Microsoft Graph v1.0 和 beta 中特定的 API 级别更改。

有关这些 API 更改的意义以及最新工具、组件、指南和教程添加项的摘要信息，请参阅 [Microsoft Graph 新增功能](whats-new-overview.md)。

## <a name="june-2020"></a>2020 年 6 月

### <a name="cloud-communications"></a>云通信
| **更改类型** | **版本**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | v1.0 | 新增了 [onlineMeeting: createOrGet](/graph/api/onlinemeeting-createorget) 方法。|
| 添加项 | v1.0 | 新增了 **externalId** 属性。 |
|添加项 | beta | 添加了指向[Get 状态](/graph/api/presence-get?view=graph-rest-beta)API 的其他路径。|
|添加 | v1.0 | 为[联机会议](/graph/api/resources/onlinemeeting)`Accept-Language`增加了可选标题。|

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version**   | **说明** |
|:---|:---|:---|
|Addition|beta|添加的新实体：<br/>[complianceManagementPartner](/graph/api/resources/intune-onboarding-compliancemanagementpartner?view=graph-rest-1.0)<br/>|
|添加|beta 版本|新增了复杂类型：<br/>[complianceManagementPartnerAssignment](/graph/api/resources/intune-onboarding-compliancemanagementpartner?view=graph-rest-1.0)<br/>|
|Addition|beta|将 **complianceManagementPartners** 导航属性添加到 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-1.0) 实体中|

### <a name="identity-and-access"></a>身份和访问
| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | beta | 添加了[连接器](/graph/api/resources/connector?view=graph-rest-beta)实体和以下操作： <br/> [获取连接器](/graph/api/connector-get?view=graph-rest-beta) <br/> [List memberOf](/graph/api/connector-list-memberof?view=graph-rest-beta) <br/> [列出连接器](/graph/api/connector-list?view=graph-rest-beta) <br/> [将连接器添加到 connectorGroup](/graph/api/connector-post-memberof?view=graph-rest-beta) |
| Addition | beta | 添加了[connectorGroup](/graph/api/resources/connectorgroup?view=graph-rest-beta)实体和以下操作： <br/> [获取 connectorGroup](/graph/api/connectorgroup-get?view=graph-rest-beta) <br/> [分配应用程序](/graph/api/connectorgroup-post-applications?view=graph-rest-beta) <br/> [列出应用程序](/graph/api/connectorgroup-list-applications?view=graph-rest-beta)  <br/> [列出 connectorGroups](/graph/api/connectorgroup-list?view=graph-rest-beta) <br/> [添加连接器](/graph/api/connectorgroup-post-members?view=graph-rest-beta) <br/> [列出连接器](/graph/api/connectorgroup-list-members?view=graph-rest-beta) <br/> [更新 connectorGroup](/graph/api/connectorgroup-update?view=graph-rest-beta) <br/> [删除 connectorGroup](/graph/api/connectorgroup-delete?view=graph-rest-beta) |
| 添加 | beta | 添加了[onPremisesPublishing](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)实体。 |
| 添加 | beta | 添加了[onPremisesPublishingSingleSignOn](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta)实体。 |
| 添加 | beta | 添加了[verifiedCustomDomainCertificatesMetadata](/graph/api/resources/verifiedcustomdomaincertificatesmetadata?view=graph-rest-beta)实体。|
| Addition | beta | 添加了[kerberosSignOnSettings](/graph/api/resources/kerberossignonsettings?view=graph-rest-beta)实体。 |
| 更改 | beta | 在[onPremisesAgent](/graph/api/resources/onpremisesagent?view=graph-rest-beta)、 [onPremisesAgentGroup](/graph/api/resources/onpremisesagentgroup?view=graph-rest-beta)和[PublishedResource](/graph/api/resources/publishedresource?view=graph-rest-beta)实体中更改了 publishingType 值从**appProxy**到**applicationProxy**。 |
| Addition | beta | 向[onPremisesPublishingProfile](/graph/api/resources/onpremisespublishingprofile?view=graph-rest-beta)实体添加了**isEnabled**属性。 |
| Addition | beta | 向 OnPremisesPublishingProfile 实体添加了作为导航属性的[连接器](/graph/api/resources/connector?view=graph-rest-beta)和[connectorGroup](/graph/api/resources/connectorgroup?view=graph-rest-beta) 。 |
| Addition | beta | 将**onPremisesPublishing**属性添加到 [application] （/graph/api/resources/application？ view = graph-rest-beta entity。 |
| Addition | beta | 添加了**OnPremisesPublishing**属性以[更新应用程序](/graph/api/application-update?view=graph-rest-beta)。 |
| Addition | beta | 添加了新资源[authenticationFlowsPolicy](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta)和[selfServiceSignUpAuthenticationFlowConfiguration](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta)以及[获取](/graph/api/authenticationflowspolicy-get?view=graph-rest-beta)和[更新](/graph/api/authenticationflowspolicy-update?view=graph-rest-beta)操作。|
| 添加项 | beta、v1.0 | 添加了对[列表对话](/graph/api/group-list-conversations)、[获取对话](/graph/api/group-get-conversation)、[列出对话线索](/graph/api/conversation-list-threads)、[获取会话线程](/graph/api/group-get-thread)和[列表线程](/graph/api/group-list-threads)api 的应用程序权限的支持。 |

### <a name="security"></a>安全性

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 | Beta 和 v1.0 | 向[alert](/graph/api/resources/alert?view=graph-rest-1.0)实体添加了以下属性： **incidentIds**、 [securityResources](/graph/api/resources/securityResource?view=graph-rest-1.0)  -  **resource**、 **resourceType**、[networkConnection](/graph/api/resources/networkconnection?view=graph-rest-1.0)  -  **sourceLocation**、 **destinationLocation**。|

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项 | beta、v1.0 | 添加了新的委派权限[AppCatalog](/graph/permissions-reference#appcatalog-resource-permissions)、[了 chatmessage](/graph/permissions-reference#chatmessage-permissions)、TeamsAppInstallation、 [ReadForUser](/graph/permissions-reference#Teams-app-installation-permissions)、 [Teams.Create](/graph/permissions-reference#teams-permissions) [TeamsAppInstallation、ReadWriteForUser](/graph/permissions-reference#Teams-app-installation-permissions)[和 TeamsAppInstallation。](/graph/permissions-reference#Teams-app-installation-permissions) |
| 添加项 | beta、v1.0 | 添加了新的应用程序权限[团队。](/graph/permissions-reference#teams-permissions) [TeamsAppInstallation、ReadForUser](/graph/permissions-reference#Teams-app-installation-permissions)、 [TeamsAppInstallation](/graph/permissions-reference#Teams-app-installation-permissions)、 [TeamsAppInstallation](/graph/permissions-reference#Teams-app-installation-permissions)。 |

### <a name="users"></a>用户

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 添加了[regionalAndLanguageSettings](/graph/api/resources/regionandlanguagesettings)实体。|
| Addition | beta | 添加了[regionalFormatOverrides](/graph/api/resources/regionalformatoverrides)复杂类型。|
| 添加项 | beta | 在[regionalAndLanguageSettings](/graph/api/resources/regionalandlanguagesettings)资源上添加了[regionalAndLanguageSettings](/graph/api/regionalandlanguagesettings-get)函数。|
| Addition | beta | 在[regionalAndLanguageSettings](/graph/api/resources/regionalandlanguagesettings)资源上添加了[regionalAndLanguageSettings](/graph/api/regionalandlanguagesettings-update)函数。|
| 更改 | beta | 向[userSettings](/graph/api/resources/userSettings)资源添加了[regionalAndLanguageSettings](/graph/resources/regionalandlanguagesettings)关系。|
| 更改 | beta | 更新了[mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta)和[regionalAndLanguageSettings](/graph/api/resources/regionalandlanguagesettings)之间的澄清的[用户](/graph/api/resources/user)资源。|


## <a name="may-2020"></a>2020 年 5 月

### <a name="calendar"></a>日历

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加 | v1.0 | V1 中可用的位置 API。 添加了[位置](/graph/api/resources/place?view=graph-rest-1.0)、[会议室](/graph/api/resources/room?view=graph-rest-1.0)、 [roomList](/graph/api/resources/room?view=graph-rest-1.0)资源以及它们的方法，以便为应用程序中的位置提供丰富的详细信息。 |

### <a name="change-notifications"></a>更改通知

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项 | beta | 为[更改通知](/graph/api/concepts/webhooks)API 添加了[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta)、 [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)和[changeNotificationEncryptedContent](/graph/api/resources/changenotificationencryptedcontent?view=graph-rest-beta)资源。 |
| Addition | v1.0 | 添加了对适用于[美国政府的 Microsoft 云中](deployments.md)[订阅](/graph/api/resources/subscription)的支持。 |


### <a name="cloud-communications--call-records"></a>云通信 | 通话记录

添加了新的 Api 和资源，用于订阅和将组织中的呼叫记录检索到1.0 版。 添加了新的列表会话 API、其他 Wi-fi 区段枚举值，以及 beta 中的其他服务角色枚举值。

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
| 添加 | v1.0 | 添加了[获取 callRecord](/graph/api/callrecords-callrecord-get?view=graph-rest-1.0) API。|
| 添加项 | v1.0 | 添加的新实体：<br /><li>[callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0)</li> <li>[Session](/graph/api/resources/callrecords-session?view=graph-rest-1.0)</li> <li>[segment](/graph/api/resources/callrecords-segment?view=graph-rest-1.0)</li>|
| 添加项 | v1.0 | 新增了复杂类型：<br /><li>[endpoint](/graph/api/resources/callrecords-endpoint?view=graph-rest-1.0)</li> <li>[participantEndpoint](/graph/api/resources/callrecords-participantendpoint?view=graph-rest-1.0)</li> <li>[serviceEndpoint](/graph/api/resources/callrecords-serviceendpoint?view=graph-rest-1.0)</li> <li>[userAgent](/graph/api/resources/callrecords-useragent?view=graph-rest-1.0)</li> <li>[serviceUserAgent](/graph/api/resources/callrecords-serviceuseragent?view=graph-rest-1.0)</li> <li>[clientUserAgent](/graph/api/resources/callrecords-clientuseragent?view=graph-rest-1.0)</li> <li>[userfeedback](/graph/api/resources/callrecords-userfeedback?view=graph-rest-1.0)</li> <li>[feedbackTokenSet](/graph/api/resources/callrecords-feedbacktokenset?view=graph-rest-1.0)</li> <li>[media](/graph/api/resources/callrecords-media?view=graph-rest-1.0)</li> <li>[mediaStream](/graph/api/resources/callrecords-mediastream?view=graph-rest-1.0)</li> <li>[networkInfo](/graph/api/resources/callrecords-networkinfo?view=graph-rest-1.0)</li> <li>[deviceInfo](/graph/api/resources/callrecords-deviceinfo?view=graph-rest-1.0)</li> <li>[failureInfo](/graph/api/resources/callrecords-failureinfo?view=graph-rest-1.0)</li> |
| 添加项 | v1.0 | 添加了对通话记录的 [webhook](webhooks.md) 订阅的支持。|
| 更改 | v1.0 | 添加 `frequency60GHz` 了并添加 `unknownFutureValue` 到**callRecords**枚举。|
| 更改 | v1.0 | 添加 `voicemail` 到**callRecords**枚举中。|
| 添加项 | v1.0 | 添加了[列表会话](/graph/api/callrecords-session-list?view=graph-rest-beta)API。 |

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
| 更改 | beta | 将 "**共享**导航" 属性的类型更改为[printer](/graph/api/resources/printer?view=graph-rest-beta) entity 上的**printerShare 集合**。 |
| 更改 | beta | 弃用了[printerShare](/graph/api/resources/printerShare?view=graph-rest-beta)实体上的**name**属性。 |
| 更改 | beta | 弃用了[printer](/graph/api/resources/printer?view=graph-rest-beta)实体上的**name**和**acceptingJobs**属性。 |
| 更改 | beta | 弃用了[打印](/graph/api/resources/print?view=graph-rest-beta)实体上的**printerShares**导航属性。<br/> 不久，URL 路径（如 "/print/printerShares/ \* "）将停止工作。 改为使用 "/print/shares/ \* "。 |
| 更改 | beta | 弃用了[printer](/graph/api/resources/printerShare?view=graph-rest-beta)实体上的**registeredBy**属性。 |
| 添加项 | beta | 在[打印](/graph/api/resources/print?view=graph-rest-beta)实体上添加了**共享**导航属性。 |
| 添加项 | beta | 向[printer](/graph/api/resources/printer?view=graph-rest-beta)实体添加了**displayName**和**isAcceptingJobs**属性。 |
| 添加项 | beta | 向[printerShare](/graph/api/resources/printerShare?view=graph-rest-beta)实体添加了属性： <br/> <ul><li>**manufacturer**</li><li>**model**</li><li>**isAcceptingJobs**</li><li>**缺省值**</li><li>**能力**</li><li>**位置**</li><li>**status**</li><li>**jobs**</li></ul> |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version**   | **说明** |
|:---|:---|:---|
|Addition|beta|添加的新实体：<br/>[featureFlightedConfiguration](/graph/api/resources/intune-deviceconfig-featureflightedconfiguration?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[deviceHealthScriptBooleanParameter](/graph/api/resources/intune-devices-devicehealthscriptbooleanparameter?view=graph-rest-beta)<br/>[deviceHealthScriptDailySchedule](/graph/api/resources/intune-devices-devicehealthscriptdailyschedule?view=graph-rest-beta)<br/>[deviceHealthScriptHourlySchedule](/graph/api/resources/intune-devices-devicehealthscripthourlyschedule?view=graph-rest-beta)<br/>[deviceHealthScriptIntegerParameter](/graph/api/resources/intune-devices-devicehealthscriptintegerparameter?view=graph-rest-beta)<br/>[deviceHealthScriptParameter](/graph/api/resources/intune-devices-devicehealthscriptparameter?view=graph-rest-beta)<br/>[deviceHealthScriptRunOnceSchedule](/graph/api/resources/intune-devices-devicehealthscriptrunonceschedule?view=graph-rest-beta)<br/>[deviceHealthScriptRunSchedule](/graph/api/resources/intune-devices-devicehealthscriptrunschedule?view=graph-rest-beta)<br/>[deviceHealthScriptStringParameter](/graph/api/resources/intune-devices-devicehealthscriptstringparameter?view=graph-rest-beta)<br/>[deviceHealthScriptTimeSchedule](/graph/api/resources/intune-devices-devicehealthscripttimeschedule?view=graph-rest-beta)<br/>[macOSAppleEventReceiver](/graph/api/resources/intune-deviceconfig-macosappleeventreceiver?view=graph-rest-beta)<br/>[macOSPrivacyAccessControlItem](/graph/api/resources/intune-deviceconfig-macosprivacyaccesscontrolitem?view=graph-rest-beta)<br/>[macOSSystemExtension](/graph/api/resources/intune-deviceconfig-macossystemextension?view=graph-rest-beta)<br/>[macOSSystemExtensionTypeMapping](/graph/api/resources/intune-deviceconfig-macossystemextensiontypemapping?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新枚举类型：<br/>[androidDeviceOwnerEnrollmentProfileType](/graph/api/resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype?view=graph-rest-beta)<br/>[deviceManagementTemplateSubtype](/graph/api/resources/intune-deviceintent-devicemanagementtemplatesubtype?view=graph-rest-beta)<br/>[joinType](/graph/api/resources/intune-devices-jointype?view=graph-rest-beta)<br/>[macOSProcessIdentifierType](/graph/api/resources/intune-deviceconfig-macosprocessidentifiertype?view=graph-rest-beta)<br/>[macOSSystemExtensionType](/graph/api/resources/intune-deviceconfig-macossystemextensiontype?view=graph-rest-beta)<br/>|
|添加项|beta|在 [mobileApp](/graph/api/resources/intune-shared-mobileapp?view=graph-rest-beta) 集合上添加了 [validateXml](/graph/api/intune-apps-mobileapp-validatexml?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) 上添加了 [createCopy](/graph/api/intune-deviceintent-devicemanagementintent-createcopy?view=graph-rest-beta) 操作 |
|删除|beta|删除了以下实体：<br/>**comanagementEligibleDeviceEntity**<br/>**comanagementEligibleSummaryEntity**<br/>|
|删除|beta|删除了以下复杂类型：<br/>**dailySchedule**<br/>**hourlySchedule**<br/>**runSchedule**<br/>|
|删除|beta|删除了以下枚举类型：<br/>**coManagementEligibleType**<br/>|
|添加项|beta|向 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **microsoftLauncherConfigurationEnabled** 和 **enrollmentProfile** 属性|
|添加项|beta|向 [deviceEnrollmentConfiguration](/graph/api/resources/intune-shared-deviceenrollmentconfiguration?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 实体添加了 **detectionScriptParameters** 和 **remediationScriptParameters** 属性|
|更改|beta|更改了 [deviceHealthScriptAssignment](/graph/api/resources/intune-devices-devicehealthscriptassignment?view=graph-rest-beta) 实体上的以下属性的类型：<br/>**runSchedule** 从 [runSchedule](/graph/api/resources/runSchedule.md?view=graph-rest-beta) 更改为 [deviceHealthScriptRunSchedule](/graph/api/resources/intune-devices-devicehealthscriptrunschedule?view=graph-rest-beta)<br/>|
|添加项|beta|向 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 实体添加了 **templateSubtype** 属性|
|添加项|beta|向 [macOSExtensionsConfiguration](/graph/api/resources/intune-deviceconfig-macosextensionsconfiguration?view=graph-rest-beta) 实体添加了 **systemExtensionsBlockOverride**、**systemExtensionsAllowedTeamIdentifiers**、**systemExtensionsAllowed** 和 **systemExtensionsAllowedTypes** 属性|
|添加项|beta|向 [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **privacyAccessControls** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **joinType** 和 **skuFamily** 属性|
|添加项|beta|向 [windowsWifiEnterpriseEAPConfiguration](/graph/api/resources/intune-deviceconfig-windowswifienterpriseeapconfiguration?view=graph-rest-beta) 实体添加了 **rootCertificateForClientValidation** 导航属性|
|添加项|beta|向 [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta) 复杂类型添加了 **operatingSystemProductType** 属性|
|添加项|beta|向 [retireScheduledManagedDevice](/graph/api/resources/intune-deviceconfig-retirescheduledmanageddevice?view=graph-rest-beta) 复杂类型添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [configurationUsage](/graph/api/resources/intune-deviceconfig-configurationusage?view=graph-rest-beta) 枚举类型添加了 **notConfigured** 成员|
|添加项|beta|向 [deviceEnrollmentType](/graph/api/resources/intune-shared-deviceenrollmenttype?view=graph-rest-beta) 枚举类型添加了 **androidEnterpriseDedicatedDevice**、**androidEnterpriseFullyManaged** 和 **androidEnterpriseCorporateWorkProfile** 成员|
|添加|beta|向 [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta) 枚举类型添加了 **syncDevice** 成员|
|添加项|v1.0|添加的新枚举类型：<br/>[managedBrowserType](/graph/api/resources/intune-mam-managedbrowsertype?view=graph-rest-1.0)<br/>|
|添加|v1.0|向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-1.0) 实体添加了 **customBrowserPackageId** 和 **customBrowserDisplayName** 属性|
|添加项|v1.0|向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-1.0) 实体添加了 **customBrowserProtocol** 属性|
|添加项|v1.0|将 **managedBrowser** 属性添加到 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0) 实体中|

### <a name="groups"></a>组

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Addition|beta|在[组](/graph/api/resources/group?view=graph-rest-beta)中添加了[evaluateDynamicMembership](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta)操作。 此外，还添加了以下支持资源类型：<ul><li>[evaluateDynamicMembershipResult](/graph/api/resources/evaluatedynamicmembershipresult?view=graph-rest-beta)</li><li>[expressionEvaluationDetails](/graph/api/resources/expressionevaluationdetails?view=graph-rest-beta)</li><li>[propertyToEvaluate](/graph/api/resources/propertytoevaluate?view=graph-rest-beta)</li></ul>|
| Addition | beta | 向 [group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了“resourceBehaviorOptions”和“resourceProvisioningOptions”属性。********|
| 添加 | v1.0 | 向[group](/graph/api/resources/group?view=graph-rest-1.0)实体添加了 **、onpremisesdomainname**、 **onPremisesNetBiosName**和**onPremisesSamAccountName**属性。|
| 添加 | v1.0 | 添加了对[由世纪互联运营的 Microsoft 云中国](deployments.md)中的**组**资源[订阅](/graph/api/resources/subscription)的支持。 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 向[riskDetection](/graph/api/resources/riskdetection?view=graph-rest-beta)和[riskyUserHistoryItem](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)资源添加了**riskEventType**属性。 使用此属性而不是**riskType**属性来检索标识保护风险检测的类型。
| 更改 | beta | 更新了 [conditionalaccessconditionset](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta) 中的 **clientAppTypes** 属性，以将 `modern` 替换为 `mobileAppsAndDesktopClients`。 已删除 `easUnsupported` 并已添加 `exchangeActiveSync`，包括 Exchange ActiveSync 支持和不支持的平台。 |
| 添加 | v1.0 | 将 Facebook 作为其他受支持的方案添加到[identityprovider.read.all](/graph/api/resources/identityprovider?view=graph-rest-1.0)资源中。 |
| Addition | beta | 添加了应用程序. All 和应用程序-读写权限。[应用程序列表](/graph/api/application-list?view=graph-rest-beta)的所有权限<br>向以下项添加了对 `$count` 、 `$search` 和 `$filter` 查询参数的支持： <br><ul><li>[列出应用程序](/graph/api/application-list?view=graph-rest-beta)</li><li>[列出设备组](/graph/api/device-list-memberof?view=graph-rest-beta)</li><li>[列出设备可传递组](/graph/api/device-list-transitivememberof?view=graph-rest-beta)</li><li>[列出设备](/graph/api/device-list?view=graph-rest-beta)</li><li>[列出组 memberOf](/graph/api/group-list-memberof?view=graph-rest-beta)</li><li>[列出组成员](/graph/api/group-list-members?view=graph-rest-beta)</li><li>[列表组可传递的 memberOf](/graph/api/group-list-transitivememberof?view=graph-rest-beta)</li><li>[列表组可传递成员](/graph/api/group-list-transitivemembers?view=graph-rest-beta)</li><li>[List groups](/graph/api/group-list?view=graph-rest-beta)</li><li>[列出 orgContacts](/graph/api/orgcontact-list?view=graph-rest-beta)</li><li>[列出 servicePrincipal memberOf](/graph/api/serviceprincipal-list-memberof?view=graph-rest-beta)</li><li>[列出 servicePrincipal 可传递的 memberOf](/graph/api/serviceprincipal-list-transitivememberof?view=graph-rest-beta)</li><li>[列出 servicePrincipals](/graph/api/serviceprincipal-list?view=graph-rest-beta)</li><li>[列出用户 memberOf](/graph/api/user-list-memberof?view=graph-rest-beta)</li><li>[列出用户可传递的 memberOf](/graph/api/user-list-transitivememberof?view=graph-rest-beta)</li><li>[List users](/graph/api/user-list?view=graph-rest-beta)</li></ul><br>添加了使用 OData 转换为以下内容的示例： <ul><li>[列出组 memberOf](/graph/api/group-list-memberof?view=graph-rest-beta)</li><li>[列出组成员](/graph/api/group-list-members?view=graph-rest-beta)</li><li>[列表组可传递的 memberOf](/graph/api/group-list-transitivememberof?view=graph-rest-beta)</li><li>[列出 servicePrincipal memberOf](/graph/api/serviceprincipal-list-memberof?view=graph-rest-beta)</li><li>[列出 servicePrincipal 可传递的 memberOf](/graph/api/serviceprincipal-list-transitivememberof?view=graph-rest-beta)</li><li>[列出用户 memberOf](/graph/api/user-list-memberof?view=graph-rest-beta)</li><li>[列出用户可传递的 memberOf](/graph/api/user-list-transitivememberof?view=graph-rest-beta)</li></ul> |
| 添加 | v1.0 | 添加了新实体类型： [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)。|
| 添加 | v1.0 | 添加了新实体类型： [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0)。|
| 添加项 | beta、v1.0 | 添加了 "仅限应用" 和 "委派" 权限[AppRoleAssignment](permissions-reference.md#application-resource-permissions)。 |
| Addition | beta | 添加了委派权限[EntitlementManagement](permissions-reference.md#entitlement-management-permissions)。 |
| Addition | beta | 添加了控制 Azure AD 中的授权设置的[authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta)资源类型。 |

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | v1.0 | 增加了对发送[频道消息](/graph/api/resources/chatmessage?view=graph-rest-1.0)和频道邮件答复的支持。|
| 添加 | v1.0 | 增加了对获取通道**的工作**的[channel](/graph/api/resources/channel?view=graph-rest-1.0)支持。|
| Addition | beta | 向[teamsAppDefinition](/graph/api/resources/teamsAppDefinition?view=graph-rest-beta)添加了**azureADAppId**属性。|
| Addition | beta | 添加了针对[特定于资源的同意](/graph/permissions-reference#teams-resource-specific-consent-permissions)的权限。|

### <a name="teamwork--shifts"></a>团队合作 | 倒班

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | v1.0 | 引入了倒班 API，包括 [shift](/graph/api/resources/shift?view=graph-rest-1.0)、[workforceintegration](/graph/api/resources/workforceintegration?view=graph-rest-1.0)和相关联的方法。|

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | v1.0 | 向[user](/graph/api/resources/user?view=graph-rest-1.0)资源添加了**externalUserState**和**externalUserStateChangeDateTime**属性。 |
| 新增 | v1.0 | 添加了对[由世纪互联运营的 Microsoft 云中国](deployments.md)**用户**资源[订阅](/graph/api/resources/subscription)的支持。 |


## <a name="april-2020"></a>2020 年 4 月

### <a name="calendar"></a>日历
| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|添加 | v1.0 | 添加了新实体 [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-1.0)。 |
|新增 | v1.0 | 添加了[获取](/graph/api/calendarpermission-get?view=graph-rest-1.0)、[更新](/graph/api/calendarpermission-update?view=graph-rest-1.0)和[删除](/graph/api/calendarpermission-delete?view=graph-rest-1.0) API 来管理[日历](/graph/api/resources/calendar?view=graph-rest-1.0)上的 [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-1.0) 资源。 |
|新增 | v1.0 | 添加了新的复杂类型 [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo?view=graph-rest-1.0)。 |
| 新增 | v1.0 | 向 [event](/graph/api/resources/event?view=graph-rest-1.0) 实体添加了“isOnlineMeeting”****、“onlineMeetingProvider”**** 和“onlineMeeting”**** 属性。 “isOnlineMeeting”**** 和“onlineMeetingProvider”**** 是事件**** 的[创建](/graph/api/user-post-events?view=graph-rest-1.0)和[更新](/graph/api/event-update?view=graph-rest-1.0)方法。 |
| 新增 | v1.0 | 向 [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) 实体添加了“defaultOnlineMeetingProviders”**** 和“allowedOnlineMeetingProviders”**** 属性。 |
| 新增 | v1.0 | 向 [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) 实体添加了“isTallyingResponses”**** 属性。 |
| 新增 | v1.0 | 向 [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) 实体添加了“isRemovable”**** 属性。 |
| 添加 | v1.0 | 向 [mailboxSettings](/graph/api/resources/mailboxSettings?view=graph-rest-1.0) 实体添加了“delegateMeetingMessageDeliveryOptions”**** 属性。 |
| 添加项 | Beta 和 v1.0          | 针对 [event](/graph/api/resources/event?view=graph-rest-1.0) 实例的[高达 150MB 的文件附件](outlook-large-attachments.md)的支持。 |
| 添加项 | beta | 添加了对[位置 API](/graph/api/resources/place?view=graph-rest-beta) 的分页支持。|

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
| Addition | beta | 向 [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) 实体添加了 **allowedGroups** 和 **allowedUsers** 属性。|
| Addition | beta | 添加了 [printIdentity](/graph/api/resources/printidentity?view=graph-rest-beta) 和 [printUserIdentity](/graph/api/resources/printuseridentity?view=graph-rest-beta) 资源类型。 |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version** | **说明** |
|:---|:---|:---|
|Addition|beta|添加的新实体：<br/>[androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration?view=graph-rest-beta)<br/>[appleExpeditedCheckinConfigurationBase](/graph/api/resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase?view=graph-rest-beta)<br/>[groupPolicyOperation](/graph/api/resources/intune-grouppolicy-grouppolicyoperation?view=graph-rest-beta)<br/>[groupPolicyUploadedDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile?view=graph-rest-beta)<br/>[iosExpeditedCheckinConfiguration](/graph/api/resources/intune-deviceconfig-iosexpeditedcheckinconfiguration?view=graph-rest-beta)<br/>[userExperienceAnalyticsScoreHistory](/graph/api/resources/intune-devices-userexperienceanalyticsscorehistory?view=graph-rest-beta)<br/>|
|Addition|beta|新增了复杂类型：<br/>[androidManagedStoreAppAssignmentSettings](/graph/api/resources/intune-apps-androidmanagedstoreappassignmentsettings?view=graph-rest-beta)<br/>[androidManagedStoreAppTrack](/graph/api/resources/intune-apps-androidmanagedstoreapptrack?view=graph-rest-beta)<br/>[appleAppListItem](/graph/api/resources/intune-deviceconfig-appleapplistitem?view=graph-rest-beta)<br/>[deviceHealthScriptRemediationHistory](/graph/api/resources/intune-devices-devicehealthscriptremediationhistory?view=graph-rest-beta)<br/>[deviceHealthScriptRemediationHistoryData](/graph/api/resources/intune-devices-devicehealthscriptremediationhistorydata?view=graph-rest-beta)<br/>[deviceManagementSettingAbstractImplementationConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingabstractimplementationconstraint?view=graph-rest-beta)<br/>[groupPolicyUploadedLanguageFile](/graph/api/resources/intune-grouppolicy-grouppolicyuploadedlanguagefile?view=graph-rest-beta)<br/>|
|Addition|beta 版本|添加的新枚举类型：<br/>[androidProfileApplicability](/graph/api/resources/intune-apps-androidprofileapplicability?view=graph-rest-beta)<br/>[groupPolicyOperationStatus](/graph/api/resources/intune-grouppolicy-grouppolicyoperationstatus?view=graph-rest-beta)<br/>[groupPolicyOperationType](/graph/api/resources/intune-grouppolicy-grouppolicyoperationtype?view=graph-rest-beta)<br/>[groupPolicyUploadedDefinitionFileStatus](/graph/api/resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus?view=graph-rest-beta)<br/>|
|Addition|beta|添加 [getAvailableExtensionProperties](o:getAvailableExtensionProperties?view=graph-rest-beta) 操作|
|添加项|beta|添加 [getObjectsById](o:getObjectsById?view=graph-rest-beta) 操作|
|添加项|beta|在 [groupPolicyUploadedDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile?view=graph-rest-beta) 上添加了 [addLanguageFiles](/graph/api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-addlanguagefiles?view=graph-rest-beta) 操作 |
|添加项|beta|在 [groupPolicyUploadedDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile?view=graph-rest-beta) 上添加了 [removeLanguageFiles](/graph/api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-removelanguagefiles?view=graph-rest-beta) 操作 |
|添加项|beta|在 [groupPolicyUploadedDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile?view=graph-rest-beta) 上添加了 [updateLanguageFiles](/graph/api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-updatelanguagefiles?view=graph-rest-beta) 操作 |
|添加项|beta|在 [groupPolicyUploadedDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile?view=graph-rest-beta) 上添加了 [uploadNewVersion](/graph/api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-uploadnewversion?view=graph-rest-beta) 操作 |
|添加项|beta|在 [groupPolicyUploadedDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile?view=graph-rest-beta) 上添加了 [remove](/graph/api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-remove?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getPolicyNonComplianceSummaryReport](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 上添加了 [getRemediationHistory](/graph/api/intune-devices-devicehealthscript-getremediationhistory?view=graph-rest-beta) 函数 |
|删除|beta|删除了以下实体：<br/>**userExperienceAnalyticsStartupScoreHistory**<br/>|
|添加项|beta|向 [androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta) 实体添加了 **profileApplicability** 属性|
|添加项|beta|向 [androidManagedStoreApp](/graph/api/resources/intune-apps-androidmanagedstoreapp?view=graph-rest-beta) 实体添加了 **appTracks** 属性|
|添加项|beta|向 [androidManagedStoreAppConfiguration](/graph/api/resources/intune-apps-androidmanagedstoreappconfiguration?view=graph-rest-beta) 实体添加了 **profileApplicability** 属性|
|添加项|beta|向 [groupPolicyObjectFile](/graph/api/resources/intune-gpanalyticsservice-grouppolicyobjectfile?view=graph-rest-beta) 实体添加了 **groupPolicyObjectId**、**ouDistinguishedName**、**createdDateTime** 和 **lastModifiedDateTime** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **specificationVersion** 属性|
|添加项|beta|向 [androidDeviceOwnerEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **derivedCredentialSettings** 导航属性|
|添加项|beta|向 [androidDeviceOwnerVpnConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownervpnconfiguration?view=graph-rest-beta) 实体添加了 **derivedCredentialSettings** 导航属性|
|Addition|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **userExperienceAnalyticsScoreHistory** 和 **groupPolicyUploadedDefinitionFiles** 导航属性|
|删除|beta|从 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体中删除了 **userExperienceAnalyticsStartupScoreHistory** 导航属性|
|添加项|beta|向 [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 复杂类型添加了 **settingInstanceId** 属性|
|添加项|beta|向 [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 复杂类型添加了 **settingInstanceId** 属性|
|添加项|beta|向 [iosAzureAdSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-iosazureadsinglesignonextension?view=graph-rest-beta) 复杂类型添加了 **enableSharedDeviceMode** 和 **configurations** 属性|
|添加项|beta|向 [managedDeviceMobileAppConfigurationSettingState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationsettingstate?view=graph-rest-beta) 复杂类型添加了 **settingInstanceId** 属性|
|添加项|beta|向 [deviceEnrollmentType](/graph/api/resources/intune-shared-deviceenrollmenttype?view=graph-rest-beta) 枚举类型添加了 **azureAdJoinUsingAzureVmExtension** 成员|
|添加项|beta|向 [policyPlatformType](/graph/api/resources/intune-shared-policyplatformtype?view=graph-rest-beta) 枚举类型添加了 **windows10XProfile** 成员|

### <a name="files"></a>文件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 在 [driveItem](/graph/api/driveitem-checkin?view=graph-rest-v1.0) 资源上添加了 [check in](/graph/api/driveitem-checkin?view=graph-rest-v1.0) 和 [check out](/graph/api/resources/driveitem?view=graph-rest-v1.0) 操作。 |
| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项        | v1.0        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 资源的 [createLink](/graph/api/driveitem-createlink?view=graph-rest-1.0) 操作上添加l了 **expirationDateTime**、**password**、**message**属性。 |
| 添加项        | v1.0        | 向 [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-1.0) 资源添加了 **preventsDownload** 属性。 |
| 添加项        | v1.0        | 向 [sharedDriveItem](/graph/api/resources/shareddriveitem?view=graph-rest-1.0) 资源添加了 **permission** 属性。 |
| 添加项        | v1.0        | 向 [permission](/graph/api/resources/permission?view=graph-rest-1.0) 资源添加了 **expirationDateTime**、**hasPassword** 和 **grantedToIdentities** 属性。 |
| 添加项        | v1.0        | 向 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 资源上的 [invite](/graph/api/driveitem-invite?view=graph-rest-1.0) 操作添加了 **expirationDateTime** 和 **password** 属性。 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version**   | **说明** |
|:---|:---|:---|
| 添加 | beta | 添加了 [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-beta)、[rbacApplicationMultiple](/graph/api/resources/rbacapplicationmultiple?view=graph-rest-beta) 和 [appScope](/graph/api/resources/appscope?view=graph-rest-beta) 以及以下操作：<br><li>[列出 unifiedRoleAssignmentMultiple](/graph/api/unifiedroleassignmentmultiple-list?view=graph-rest-beta)</li><li>[获取 unifiedRoleAssignmentMultiple](/graph/api/unifiedroleassignmentmultiple-get?view=graph-rest-beta)</li><li>[创建 unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple-post?view=graph-rest-beta)</li><li>[更新 unifiedRoleAssignmentMultiple](/graph/api/unifiedroleassignmentmultiple-update?view=graph-rest-beta)</li><li>[删除 unifiedRoleAssignmentMultiple](/graph/api/unifiedroleassignmentmultiple-delete?view=graph-rest-beta)</li>. |
| 新增 | v1.0 | 增加了 [应用 delta 查询](/graph/api/application-delta?view=graph-rest-1.0)支持。|
| Addition | beta | 增加了 [administrativeUnits delta 查询](/graph/api/administrativeunit-delta?view=graph-rest-beta)支持。|
| Addition | beta | 增加了 [oAuth2PermissionGrant 查询](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta)支持。|
| 新增 | v1.0 | 键入的策略资源归组在 [policies](/graph/api/resources/policy-overview?view=graph-rest-1.0) URL 段下。 此更新添加 5 个类型的策略资源： <br> <li>[activityBasedTimeoutPolicies](/graph/api/resources/activityBasedTimeoutPolicy?view=graph-rest-1.0)</li> <li>[claimsMappingPolicies](/graph/api/resources/claimsMappingPolicy?view=graph-rest-1.0) </li> <li>[homeRealmDiscoveryPolicies](/graph/api/resources/homeRealmDiscoveryPolicy?view=graph-rest-1.0) </li> <li>[tokenLifetimePolicies](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0) 和 </li> <li>[tokenIssuancePolicies](/graph/api/resources/tokenissuancepolicy?view=graph-rest-1.0)</li>|
| 新增 | v1.0 | 对于支持基于活动的超时功能的应用程序，添加的 [activityBasedTimeoutPolicy](/graph/api/resources/activityBasedTimeoutPolicy?view=graph-rest-1.0) 资源类型，可在一段时间后控制自动注销 Web 会话。|
| 新增 | v1.0 |添加了 [claimsMappingPolicy](/graph/api/resources/claimsMappingPolicy?view=graph-rest-1.0) 资源类型，它控制用于 WS-AT、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射，适用于向特定应用程序发出的令牌。|
| 新增 | v1.0 | 添加了 [homeRealmDiscoveryPolicy](/graph/api/resources/homeRealmDiscoveryPolicy?view=graph-rest-1.0) 资源类型，它控制联盟用户的 Azure Active Directory 身份验证行为，尤其适用于联合域中的自动加速和用户身份验证限制。 |
| 新增 | v1.0 | 添加了 [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0) 资源类型，它控制用于访问受保护资源的访问令牌的生存期持续时间。|
| 新增 | v1.0 | 添加了 [tokenIssuancePolicy](/graph/api/resources/tokenissuancepolicy?view=graph-rest-1.0) 资源类型，它控制由 Azure AD 颁发的 SAML 令牌的特征。 它允许你设置用于颁发 SAML 令牌的签名算法、签名选项或 SAML 令牌版本。|
| Addition | beta | 增加了 [authenticationMethod](/graph/api/resources/authenticationmethod?view=graph-rest-beta)、[passwordAuthenticationMethod](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta)、和 [phoneAuthenticationMethod](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta) 资源和相关方法。
| Addition | beta | 向 [group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了 **createdByAppId** 属性。|

### <a name="mail"></a>邮件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项        | V1.0          | 向 [message](/graph/api/resources/message?view=graph-rest-1.0) 实例[添加高达 150MB 的文件附件](outlook-large-attachments.md)。 |
| 添加项        | V1.0          | [attachmentItem](/graph/api/resources/attachmentitem?view=graph-rest-1.0) 复杂类型、[attachment](/graph/api/resources/attachment?view=graph-rest-1.0) 实体的 [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) 操作和 **attachmentType** 枚举。 |
| 更改项         | V1.0          | 扩展了 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 所使用的现有 [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-1.0) 实体，以使其也适用于 **attachment**。 |

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | beta | 新增了新资源类型 [relyingPartyDetailedSummary](/graph/api/resources/relyingpartydetailedsummary?view=graph-rest-beta)。 此资源类型支持[列出](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta) Active Directory 联合身份验证服务中配置的依赖方。|

### <a name="reports--office-365-usage-reports"></a>报告 | Office 365 使用率报告

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 向 [getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta) API CSV 实体添加了 **Meeting Created** 和 **Meeting Interacted** 属性。 |
| 添加 | Beta | 向 [getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) API CSV 实体添加了 **Meeting Created** 和 **Meeting Interacted** 属性。 |
| 添加 | Beta | 向 [getEmailActivityuserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta) API CSV 实体添加了 **Meeting Created** 和 **Meeting Interacted** 属性。 |

### <a name="sites-and-lists"></a>站点和列表

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | beta        | 向 **followedSites** 导航属性添加了 [user](/graph/api/resources/user?view=graph-rest-beta) 实体， 以[列出登录用户关注的网站](/graph/api/sites-list-followed?view=graph-rest-beta)。 |
| 新增        | v1.0        | 向 **followedSites** 导航属性添加了 [user](/graph/api/resources/user?view=graph-rest-1.0) 实体， 以[列出登录用户关注的网站](/graph/api/sites-list-followed?view=graph-rest-1.0)。 |
| 新增        | v1.0        | 向 [siteCollection](/graph/api/resources/sitecollection?view=graph-rest-1.0) 资源添加了 **dataLocatonCode** 属性。 |
| 添加项        | v1.0        | 向 [sharepointIds](/graph/api/resources/sharepointids?view=graph-rest-1.0) 资源添加了 **tenantId** 属性。 |


## <a name="march-2020"></a>2020 年 3 月

### <a name="calendar"></a>日历

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 向 [日历](/graph/api/resources/calendar?view=graph-rest-beta) 实体添加了 **calendarGroupId** 属性。 |
| Addition | Beta | 已向 [事件](/graph/api/resources/event?view=graph-rest-beta) 实体中添加了 **isDraft** 属性。 |

### <a name="cloud-communications--call"></a>云通信 | 呼叫

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加|v1.0|已将新属性 [initiator](/graph/api/resources/recordinginfo?view=graph-rest-1.0) 添加至 **recordingInfo** 复杂类型。
|新增|v1.0|新增了复杂类型：<br/>[recordingInfo](/graph/api/resources/recordinginfo?view=graph-rest-1.0)<br/>[callRoute](/graph/api/resources/callRoute?view=graph-rest-1.0)<br/>[incomingContext](/graph/api/resources/incomingcontext?view=graph-rest-1.0)
|新增|v1.0|已将新属性 **recordingInfo** 添加至 [participant](/graph/api/resources/participant?view=graph-rest-1.0) 实体。
|新增|v1.0|已将新属性 [recordingStatus](/graph/api/resources/recordinginfo?view=graph-rest-1.0) 添加至 **recordingInfo** 复杂类型。
|新增|v1.0|已将新操作 [updateRecordingStatus](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0) 添加至 [call](/graph/api/resources/call?view=graph-rest-1.0) 实体。
|新增|v1.0|已将新属性 **endpointType** 添加至 [recordingInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0) 复杂类型。
|新增|v1.0|已将新属性 **countryCode** 添加至 [recordingInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0) 复杂类型。
|新增|v1.0|已将新属性 **incomingContext** 添加到 [call](/graph/api/resources/call?view=graph-rest-1.0) 实体。
|新增|v1.0|已将新属性 **sourceParticipantId** 添加到 [incomingContext](/graph/api/resources/incomingcontext?view=graph-rest-1.0) 复杂类型。
|新增|v1.0|已将新属性 **observedParticipantId** 添加到 [incomingContext](/graph/api/resources/incomingcontext?view=graph-rest-1.0) 复杂类型。
|新增|v1.0|已将新属性 **onBehalfOf** 添加到 [incomingContext](/graph/api/resources/incomingcontext?view=graph-rest-1.0) 复杂类型。
|新增|v1.0|已将新属性 **transferor** 添加到 [incomingContext](/graph/api/resources/incomingcontext?view=graph-rest-1.0) 复杂类型。
|Addition|v1.0|已将新属性 **CallRoutes** 添加到 [call](/graph/api/resources/call?view=graph-rest-1.0) 实体。
|添加项|v1.0|已将新属性 **final** 添加到 [callRoute](/graph/api/resources/callroute?view=graph-rest-1.0) 实体。
|Addition|v1.0|已将新属性 **original** 添加到 [callRoute](/graph/api/resources/callroute?view=graph-rest-1.0) 复杂类型。
|新增|v1.0|已将新属性 **routingType** 添加到 [callRoute](/graph/api/resources/callroute?view=graph-rest-1.0) 复杂类型。
|添加项|Beta 和 v1.0|在 [call](/graph/api/resources/call) 集合上添加了 [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality) 函数。|
|添加项|Beta 和 v1.0|向 [call](/graph/api/resources/call) 实体添加了 **callChainId** 属性。|
|添加项|Beta 和 v1.0|新增了复杂类型：<br/>[teleconferenceDeviceQuality](/graph/api/resources/teleconferencedevicequality)<br/>[teleconferenceDeviceMediaQuality](/graph/api/resources/teleconferencedevicemediaquality)<br/>[teleconferenceDeviceAudioQuality](/graph/api/resources/teleconferencedeviceaudioquality)<br/>[teleconferenceDeviceVideoQuality](/graph/api/resources/teleconferencedevicevideoquality)<br/>[teleconferenceDeviceScreenSharingQuality](/graph/api/resources/teleconferencedevicescreensharingquality)。|

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议

| **更改类型** | **Version** | **说明** |
|:---|:---|:---|
| 添加 | beta | 新增了 [onlineMeeting: createOrGet](/graph/api/onlinemeeting-createorget) 方法。|
| Addition | beta | 向 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta) 添加了可选的 **externalId** 属性。 |
|Addition|beta|为[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)`Accept-Language`增加了可选标题。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version** | **说明** |
|:---|:---|:---|
|添加|beta|已将 **executionFrequency**、 **retryCount** 和 **blockExecutionNotifications** 属性添加至 [deviceShellScript](/graph/api/resources/intune-devices-deviceshellscript?view=graph-rest-beta) 实体。|
|添加项|beta|添加的新实体：<br/>[deviceManagementAutopilotPolicyStatusDetail](/graph/api/resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail?view=graph-rest-beta)<br/>[groupPolicyCategory](/graph/api/resources/intune-grouppolicy-grouppolicycategory?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[configurationManagerActionResult](/graph/api/resources/intune-devices-configurationmanageractionresult?view=graph-rest-beta)<br/>[deviceHealthScriptRemediationSummary](/graph/api/resources/intune-devices-devicehealthscriptremediationsummary?view=graph-rest-beta)<br/>[deviceManagementSettingSddlConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingsddlconstraint?view=graph-rest-beta)<br/>[iosAzureAdSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-iosazureadsinglesignonextension?view=graph-rest-beta)<br/>[macOSAssociatedDomainsKeyValuePair](/graph/api/resources/intune-deviceconfig-macosassociateddomainskeyvaluepair?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新枚举类型：<br/>[configurationManagerActionDeliveryStatus](/graph/api/resources/intune-devices-configurationmanageractiondeliverystatus?view=graph-rest-beta)<br/>[deviceManagementAutopilotPolicyComplianceStatus](/graph/api/resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus?view=graph-rest-beta)<br/>[deviceManagementAutopilotPolicyType](/graph/api/resources/intune-troubleshooting-devicemanagementautopilotpolicytype?view=graph-rest-beta)<br/>[win32LobAppDeliveryOptimizationPriority](/graph/api/resources/intune-apps-win32lobappdeliveryoptimizationpriority?view=graph-rest-beta)<br/>|
|添加项|beta|添加 [getAvailableExtensionProperties](o:getAvailableExtensionProperties?view=graph-rest-beta) 操作|
|添加项|beta|添加 [getObjectsById](o:getObjectsById?view=graph-rest-beta) 操作|
|添加项|beta|在 [applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-beta) 上添加了 [generateApplePushNotificationCertificateSigningRequest](/graph/api/intune-devices-applepushnotificationcertificate-generateapplepushnotificationcertificatesigningrequest?view=graph-rest-beta?view=graph-rest-beta) 操作 |
|添加项|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 上添加了 [generateEncryptionPublicKey](/graph/api/intune-enrollment-deponboardingsetting-generateencryptionpublickey?view=graph-rest-beta?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getSettingNonComplianceReport](/graph/api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport?view=graph-rest-beta?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 集合上添加了 [getRemediationSummary](o:getRemediationSummary:Collection(microsoft.graph.deviceHealthScript?view=graph-rest-beta)?view=graph-rest-beta) 函数 |
|删除|beta|删除了以下复杂类型：<br/>**groupPolicyObjectFile**<br/>|
|删除|beta|在 [groupPolicyMigrationReport](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreport?view=graph-rest-beta) 集合上删除了 [createMigrationReport](o:createMigrationReport:Collection(microsoft.graph.groupPolicyMigrationReport?view=graph-rest-beta)?view=graph-rest-beta) 操作 |
|删除|beta|从 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体中删除了 **groupPolicyObjectFiles** 属性|
|添加项|beta|向 [deviceManagementAutopilotEvent](/graph/api/resources/intune-troubleshooting-devicemanagementautopilotevent?view=graph-rest-beta) 实体添加了 **deviceId** 属性|
|添加项|beta|向 [groupPolicyDefinition](/graph/api/resources/intune-grouppolicy-grouppolicydefinition?view=graph-rest-beta) 实体添加了 **groupPolicyCategoryId** 属性|
|添加项|beta|向 [groupPolicySettingMapping](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingmapping?view=graph-rest-beta) 实体添加了 **intuneSettingDefinitionId** 属性|
|添加项|beta|向 [macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **fileVaultHidePersonalRecoveryKey**、**advancedThreatProtectionRealTime**、**advancedThreatProtectionCloudDelivered**、**advancedThreatProtectionAutomaticSampleSubmission**、**advancedThreatProtectionDiagnosticDataCollection**、**advancedThreatProtectionExcludedFolders**、**advancedThreatProtectionExcludedFiles**、**advancedThreatProtectionExcludedExtensions** 和 **advancedThreatProtectionExcludedProcesses** 属性|
|添加项|beta|向 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 实体添加了 **directorySizeQuota** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **defenderAllowScanArchiveFiles**、**defenderAllowBehaviorMonitoring**、**defenderAllowCloudProtection**、**defenderAllowScanRemovableDrivesDuringFullScan**、**defenderAllowScanDownloads**、**defenderAllowIntrusionPreventionSystem**、**defenderAllowOnAccessProtection**、**defenderAllowRealTimeMonitoring**、**defenderAllowScanNetworkFiles**、**defenderAllowScanScriptsLoadedInInternetExplorer**、**defenderAllowEndUserAccess** 和 **defenderSignatureUpdateIntervalInHours** 属性|
|更改|beta|更改了 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体上的以下属性：<br/>将 **defenderBlockEndUserAccess** 从必填更改为可选<br/>将 **defenderCheckForSignaturesBeforeRunningScan** 从必填更改为可选<br/>将 **defenderCloudBlockLevel** 从必填更改为可选<br/>将 **defenderDisableBehaviorMonitoring** 从必填更改为可选<br/>将 **defenderDisableCatchupFullScan** 从必填更改为可选<br/>将 **defenderDisableCatchupQuickScan** 从必填更改为可选<br/>将 **defenderDisableCloudProtection** 从必填更改为可选<br/>将 **defenderDisableIntrusionPreventionSystem** 从必填更改为可选<br/>将 **defenderDisableOnAccessProtection** 从必填更改为可选<br/>将 **defenderDisableRealTimeMonitoring** 从必填更改为可选<br/>将 **defenderDisableScanArchiveFiles** 从必填更改为可选<br/>将 **defenderDisableScanDownloads** 从必填更改为可选<br/>将 **defenderDisableScanNetworkFiles** 从必填更改为可选<br/>将 **defenderDisableScanRemovableDrivesDuringFullScan** 从必填更改为可选<br/>将 **defenderDisableScanScriptsLoadedInInternetExplorer** 从必填更改为可选<br/>将 **defenderEnableLowCpuPriority** 从必填更改为可选<br/>将 **defenderEnableScanIncomingMail** 从必填更改为可选<br/>将 **defenderEnableScanMappedNetworkDrivesDuringFullScan** 从必填更改为可选<br/>将 **defenderPotentiallyUnwantedAppAction** 从必填更改为可选<br/>将 **defenderScanDirection** 从必填更改为可选<br/>将 **defenderScanType** 从必填更改为可选<br/>将 **defenderScheduledScanDay** 从必填更改为可选<br/>将 **defenderSubmitSamplesConsentType** 从必填更改为可选<br/>|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **findMyFiles**、**activateAppsWithVoice** 和 **configureTimeZone** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **groupPolicyCategories** 导航属性|
|添加项|beta|向 [deviceManagementAutopilotEvent](/graph/api/resources/intune-troubleshooting-devicemanagementautopilotevent?view=graph-rest-beta) 实体添加了 **policyStatusDetails** 导航属性|
|添加项|beta|向 [groupPolicyDefinition](/graph/api/resources/intune-grouppolicy-grouppolicydefinition?view=graph-rest-beta) 实体添加了 **category** 导航属性|
|添加项|beta|向 [configurationManagerClientInformation](/graph/api/resources/intune-devices-configurationmanagerclientinformation?view=graph-rest-beta) 复杂类型添加了 **isBlocked** 属性|
|添加项|beta|向 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型添加了 **ignoreDevicesForUnsupportedSettingsEnabled** 属性|
|添加项|beta|向 [win32LobAppAssignmentSettings](/graph/api/resources/intune-apps-win32lobappassignmentsettings?view=graph-rest-beta) 复杂类型添加了 **deliveryOptimizationPriority** 属性|
|添加项|beta|向 [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-beta) 枚举类型添加了 **deviceOsHigherThanDesiredOsVersion** 成员。 |

### <a name="files"></a>文件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | Beta 和 v1.0 | 已将 **image** 和 **video** 属性添加至 [remoteItem](/graph/api/resources/remoteitem?view=graph-rest-1.0) 资源。 这些属性可在组合展开功能时，允许检索媒体类型缩略图。  |
| 新增 | v1.0 | 向 [permission](/graph/api/resources/permission?view=graph-rest-1.0) 实体添加了 **grant** 操作。 |
| 新增        | v1.0        | 向 [drive](/graph/api/resources/drive?view=graph-rest-v1.0) 实体添加了 **following** 导航属性。 |
| Addition        | v1.0        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-v1.0) 上添加了 [follow](/graph/api/driveitem-follow?view=graph-rest-v1.0) 操作。 |
| Addition        | v1.0        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-v1.0) 上添加了 [unfollow](/graph/api/driveitem-unfollow?view=graph-rest-v1.0) 操作。 |


### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version**   | **说明** |
|:---|:---|:---|
| 添加 | Beta 和 v1.0 | 已将 **authenticationRequirement** 属性和 **riskEventTypes_v2**属性添加至 [signin](/graph/api/resources/signin?view=graph-rest-1.0) 实体。 |
| 添加项 | Beta 和 v1.0 | 增加了 [orgContact delta 查询](/graph/api/orgcontact-delta?view=graph-rest-1.0)支持。|
| 新增 | v1.0 | 添加了新的用户权限 [User.ManageIdentities.All](/graph/permissions-reference#user-permissions)。|
| 添加项 | beta | 向 [Privileged Identity Management - Azure 资源](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) 添加了 PrivilegedAccess.Read.AzureResources 应用程序权限。 |
| 添加项 | beta | 添加了 [Auditlogs.Read.All](/graph/permissions-reference#user-permissions) 权限，用于列出用户的登录活动。|
| 添加项 | beta | 添加了 [identitySecurityDefaultsEnforcementPolicy API](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta)，它表示 Azure Active Directory 安全默认值策略。|
| 添加项 | beta | 已将 `$top` 和 `$skiptoken` 过滤器支持添加至 [List provisioningObjectSummary](/api-reference/beta/api/provisioningobjectsummary-list) 方法的支持分页上。 |

### <a name="identity-and-access--conditional-access"></a>身份和访问 | 条件访问

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 更改 | beta | 将条件访问 API 更新为使用 /identity/ 段；例如，/beta/identity/conditionalAccess/policies。|
| 添加项 | beta | 向 [conditionalaccessconditionset](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta) 实体添加了 **devices** 属性。 |

### <a name="reports--office-365-usage-reports"></a>报告 | Office 365 使用率报告

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 更改          | Beta 和 v1.0  | 为了使委派权限允许应用代表用户读取 Office 365 服务使用情况报告，已将 Teams 服务管理员和 Teams 通信管理员添加为接受的用户角色。 有关更多详细信息，请参阅[授权 API 读取 Office 365 使用情况报告](reportroot-authorization.md)。|
| 添加项        | Beta  | 向 [yammerGroupsActivityDetail](/graph/api/resources/yammerGroupsActivityDetail?view=graph-rest-beta) 实体添加了 **networkDisplayName** 属性。|

### <a name="search"></a>搜索

| 更改类型 | 版本 | 说明                                                                                                                                               |
|-------------|---------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| 更改      | beta    | [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) 资源已遭弃用。                                                  |
| 更改      | beta    | [externalItem](/graph/api/resources/externalfile?view=graph-rest-beta) 资源现在支持更新 **content** 和 **properties** 属性。      |
| 更改      | beta    | 现在，对 [externalItem](/graph/api/resources/externalfile?view=graph-rest-beta) 资源执行的操作在受到限制时返回 `Retry-After` 标头。 |

### <a name="sites"></a>网站

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :-------------------------------------- |
| 添加项        | v1.0        | 向 [user](/graph/api/resources/user?view=graph-rest-1.0) 实体添加了 [followSite](/graph/api/site-follow?view=graph-rest-1.0) 导航属性。 |
| 添加项        | v1.0        | 向 [user](/graph/api/resources/user?view=graph-rest-1.0) 实体添加了 [unfollowSite](/graph/api/site-unfollow?view=graph-rest-1.0) 导航属性。 |
| 添加项        | v1.0       | 向 [list](/graph/api/resources/list?view=graph-rest-1.0) 实体添加了 **subscriptions** 导航属性。 |

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | Beta |已将新属性 **supportedEntities** 添加到 [workforceintegration](/graph/api/resources/workforceintegration?view=graph-rest-beta) 实体。|
| 添加项 | v1.0 | 添加了新实体 [teamwork](/graph/api/resources/teamwork?view=graph-rest-1.0)。
| 添加项 | Beta | 向 API 添加了对 ChannelMessage.Read.All 的支持，以读取频道中的 [chatMessages](/graph/api/resources/chatmessage?view=graph-rest-beta)。 |

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印

新增了 API 和资源，用于使用通用打印服务来管理和执行打印机打印。

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
| 添加项 | beta | 添加了 [archivedPrintJob](/graph/api/resources/archivedprintjob) 实体。|
| 添加项 | beta | 添加了 [deviceHealth](/graph/api/resources/devicehealth) 复杂类型。|
| 添加项 | beta | 添加了 [integerRange](/graph/api/resources/integerrange) 复杂类型。|
| 添加项 | beta | 添加了 [print](/graph/api/resources/print) 实体。|
| 添加项 | beta | 添加了 [printConnector](/graph/api/resources/printconnector) 实体。|
| 添加项 | beta | 添加了 [printDocument](/graph/api/resources/printdocument) 实体。|
| 添加项 | beta | 添加了 [printer](/graph/api/resources/printer) 实体。|
| 添加项 | beta | 添加了 [printerCapabilities](/graph/api/resources/printercapabilities) 复杂类型。|
| 添加项 | beta | 添加了 [printerDefaults](/graph/api/resources/printerdefaults) 复杂类型。|
| 添加项 | beta | 添加了 [printerDocumentConfiguration](/graph/api/resources/printerdocumentconfiguration) 复杂类型。|
| 添加项 | beta | 添加了 [printerLocation](/graph/api/resources/printerlocation) 复杂类型。|
| 添加项 | beta | 添加了 [printerShare](/graph/api/resources/printershare) 实体。|
| 添加项 | beta | 添加了 [printerStatus](/graph/api/resources/printerstatus) 复杂类型。|
| 添加项 | beta | 添加了 [printJob](/graph/api/resources/printJob) 实体。|
| 添加项 | beta | 添加了 [printJobStatus](/graph/api/resources/printjobstatus) 复杂类型。|
| 添加项 | beta | 添加了 [printPageRange](/graph/api/resources/printpagerange) 复杂类型。|
| 添加项 | beta | 添加了 [printService](/graph/api/resources/printpagerange) 实体。|
| 添加项 | beta | 添加了 [printServiceEndpoint](/graph/api/resources/printserviceendpoint) 实体。|
| 添加项 | beta | 添加了 [printSettings](/graph/api/resources/printsettings) 复杂类型。|
| 添加项 | beta | 添加了 [printUsageSummaryByPrinter](/graph/api/resources/printusagesummarybyprinter) 实体。|
| 添加项 | beta | 添加了 [printUsageSummaryByUser](/graph/api/resources/printusagesummarybyuser) 实体。|


## <a name="february-2020"></a>2020 年 2 月

### <a name="cloud-communications--call"></a>云通信 | 呼叫

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项|beta|向 [recordingInfo](/graph/api/resources/recordinginfo?view=graph-rest-beta) 复杂类型新增了“ **发起程序**”属性。

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录

添加了用于订阅和检索组织中的通话记录的新 API 和资源。

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
| 添加 | beta | 添加了[获取 callRecord](/graph/api/callrecords-callrecord-get?view=graph-rest-beta) API。|
| 添加项 | beta | 添加的新实体：<br /><li>[callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta)</li> <li>[Session](/graph/api/resources/callrecords-session?view=graph-rest-beta)</li> <li>[segment](/graph/api/resources/callrecords-segment?view=graph-rest-beta)</li>|
| 添加项 | beta | 新增了复杂类型：<br /><li>[endpoint](/graph/api/resources/callrecords-endpoint?view=graph-rest-beta)</li> <li>[participantEndpoint](/graph/api/resources/callrecords-participantendpoint?view=graph-rest-beta)</li> <li>[serviceEndpoint](/graph/api/resources/callrecords-serviceendpoint?view=graph-rest-beta)</li> <li>[userAgent](/graph/api/resources/callrecords-useragent?view=graph-rest-beta)</li> <li>[serviceUserAgent](/graph/api/resources/callrecords-serviceuseragent?view=graph-rest-beta)</li> <li>[clientUserAgent](/graph/api/resources/callrecords-clientuseragent?view=graph-rest-beta)</li> <li>[userfeedback](/graph/api/resources/callrecords-userfeedback?view=graph-rest-beta)</li> <li>[feedbackTokenSet](/graph/api/resources/callrecords-feedbacktokenset?view=graph-rest-beta)</li> <li>[media](/graph/api/resources/callrecords-media?view=graph-rest-beta)</li> <li>[mediaStream](/graph/api/resources/callrecords-mediastream?view=graph-rest-beta)</li> <li>[networkInfo](/graph/api/resources/callrecords-networkinfo?view=graph-rest-beta)</li> <li>[deviceInfo](/graph/api/resources/callrecords-deviceinfo?view=graph-rest-beta)</li> <li>[failureInfo](/graph/api/resources/callrecords-failureinfo?view=graph-rest-beta)</li> |
| 添加项 | beta | 添加了对通话记录的 [webhook](webhooks.md) 订阅的支持。|

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version** | **说明** |
|:---|:---|:---|
|添加|beta|添加的新实体：<br/>[macOSMdatpApp](/graph/api/resources/intune-apps-macosmdatpapp)<br/>[unsupportedGroupPolicyExtension](/graph/api/resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension)<br/>[userExperienceAnalyticsDeviceStartupProcess](/graph/api/resources/intune-devices-userexperienceanalyticsdevicestartupprocess)<br/>[userExperienceAnalyticsDeviceStartupProcessPerformance](/graph/api/resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance)<br/>|
|添加项|beta|新增了复杂类型：<br/>[customUpdateTimeWindow](/graph/api/resources/intune-deviceconfig-customupdatetimewindow)<br/>[iosAvailableUpdateVersion](/graph/api/resources/intune-softwareupdate-iosavailableupdateversion)<br/>[managedDeviceSummarizedAppState](/graph/api/resources/intune-troubleshooting-manageddevicesummarizedappstate)<br/>|
|添加项|beta 版本|添加的新枚举类型：<br/>[enrollmentAvailabilityOptions](/graph/api/resources/intune-shared-enrollmentavailabilityoptions)<br/>[globalDeviceHealthScriptState](/graph/api/resources/intune-devices-globaldevicehealthscriptstate)<br/>[iosSoftwareUpdateScheduleType](/graph/api/resources/intune-deviceconfig-iossoftwareupdatescheduletype)<br/>|
|添加项|beta|在 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript) 上添加了 [updateGlobalScript](/graph/api/intune-devices-devicehealthscript-updateglobalscript) 操作 |
|添加项|beta|在 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript) 上添加了 [getGlobalScriptHighestAvailableVersion](/graph/api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion) 操作 |
|添加项|beta|在 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript) 集合上添加了 [enableGlobalScripts](/graph/api/intune-devices-devicehealthscript-enableglobalscripts) 操作 |
|添加项|beta|在 [user](/graph/api/resources/intune-shared-user) 上添加了 [getManagedDevicesWithFailedOrPendingApps](/graph/api/intune-troubleshooting-user-getmanageddeviceswithfailedorpendingapps) 函数 |
|添加项|beta|在 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript) 集合上添加了 [areGlobalScriptsAvailable](/graph/api/intune-devices-devicehealthscript-areglobalscriptsavailable) 函数 |
|删除|beta|删除了以下枚举类型：<br/>**logLevel**<br/>|
|添加项|beta|向 [applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate) 实体添加了 **certificateSerialNumber** 属性|
|添加项|beta|向 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript) 实体添加了 **isGlobalScript** 和 **highestAvailableVersion** 属性|
|添加项|beta|向 [deviceManagementSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementsettingcategory) 实体添加了 **hasRequiredSetting** 属性|
|添加项|beta|向 [intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile) 实体添加了 **sendDeviceOwnershipChangePushNotification**、**enrollmentAvailability** 和 **roleScopeTagIds** 属性|
|添加项|beta|向 [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration) 实体添加了 **updateScheduleType** 和 **customUpdateTimeWindows** 属性|
|添加项|beta|向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection) 实体添加了 **appActionIfUnableToAuthenticateUser** 属性|
|添加项|beta|向 [termsAndConditionsAcceptanceStatus](/graph/api/resources/intune-companyterms-termsandconditionsacceptancestatus) 实体添加了 **userPrincipalName** 属性|
|添加项|beta|向 [userExperienceAnalyticsDevicePerformance](/graph/api/resources/intune-devices-userexperienceanalyticsdeviceperformance) 实体添加了 **responsiveDesktopTimeInMs** 属性|
|添加项|beta|向 [userExperienceAnalyticsDeviceStartupHistory](/graph/api/resources/intune-devices-userexperienceanalyticsdevicestartuphistory) 实体添加了 **responsiveDesktopTimeInMs** 属性|
|添加项|beta|向 [win32LobApp](/graph/api/resources/intune-apps-win32lobapp) 实体添加了 **Installlanguage.xml** 属性|
|添加项|beta|向 [windowsMicrosoftEdgeApp](/graph/api/resources/intune-apps-windowsmicrosoftedgeapp) 实体中添加了 **displayLanguageLocale** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement) 实体添加了 **userExperienceAnalyticsDeviceStartupProcesses**、**userExperienceAnalyticsDeviceStartupProcessPerformance** 和 **userExperienceAnalyticsStartupScoreHistory** 导航属性|
|添加项|beta|向 [groupPolicyMigrationReport](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreport) 实体添加了 **unsupportedGroupPolicyExtensions** 导航属性|
|添加项|beta|向 [deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary) 复杂类型添加了 **configMgrDeviceCount** 属性|
|添加项|beta|向 [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand) 实体添加了 **roleScopeTagIds**、**sendDeviceOwnershipChangePushNotification** 和 **enrollmentAvailability** 属性|
|添加项|beta|向 [mobileAppTroubleshootingHistoryItem](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem) 复杂类型添加了 **troubleshootingErrorDetails** 属性|
|添加项|beta|向 [deviceManagementDerivedCredentialIssuer](/graph/api/resources/intune-rapolicy-devicemanagementderivedcredentialissuer) 枚举类型添加了 **xTec** 成员|
|添加项|beta|向 [deviceType](/graph/api/resources/intune-deviceconfig-devicetype) 枚举类型添加了 **windows10x** 成员|
|添加项|beta|向 [managementAgentType](/graph/api/resources/intune-deviceconfig-managementagenttype) 枚举类型添加了 **windowsManagementCloudApi** 成员|

### <a name="groups"></a>组

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | v1.0 | 添加了 [group: assignLicense API](/graph/api/group-assignlicense?view=graph-rest-1.0)，它可用于为[组](/graph/api/resources/group?view=graph-rest-1.0)分配许可证。 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
| 添加 | Beta 和 v1.0 | 向 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 实体中添加了 **latestSupportedTlsVersion** 属性。 指定通知终结点支持的最新 TLS 版本。 允许订阅者在有限的时间段内使用过时的 TLS 版本。 有关详细信息，请参阅 [Microsoft Graph 订阅 - 弃用 TLS 1.0 和 1.1](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/)。
| 更改 | beta |现有策略集将替换为[策略](/graph/api/resources/policy-overview?view=graph-rest-beta) URL 段。 键入的策略资源现在在“策略”段下分组，详见“[此博客文章](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/)”中的说明。 此更新添加 4 个类型的策略资源： <br> <li>[activityBasedTimeoutPolicies](/graph/api/resources/activityBasedTimeoutPolicy?view=graph-rest-beta)</li> <li>[claimsMappingPolicies](/graph/api/resources/claimsMappingPolicy?view=graph-rest-beta) </li> <li>[homeRealmDiscoveryPolicies](/graph/api/resources/homeRealmDiscoveryPolicy?view=graph-rest-beta) 和 </li> <li>[tokenLifetimePolicies](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta)</li> |
| 添加项 | beta | 对于支持基于活动的超时功能的应用程序，添加的 [activityBasedTimeoutPolicy](/graph/api/resources/activityBasedTimeoutPolicy?view=graph-rest-beta) 资源类型控制着一段时间不活动后 Web 会话的自动注销。|
| 添加项 | beta |添加了 [claimsMappingPolicy](/graph/api/resources/claimsMappingPolicy?view=graph-rest-beta) 资源类型，它控制用于 WS-AT、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射，适用于向特定应用程序发出的令牌。|
| 添加项 | beta | 添加了 [homeRealmDiscoveryPolicy](/graph/api/resources/homeRealmDiscoveryPolicy?view=graph-rest-beta) 资源类型，它控制联盟用户的 Azure Active Directory 身份验证行为，尤其适用于联合域中的自动加速和用户身份验证限制。 |
| 添加项 | beta | 添加了 [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta) 资源类型，它控制用于访问受保护资源的访问令牌的生存期持续时间。|
| 添加项 | beta | 添加了 [tokenIssuancePolicy](/graph/api/resources/tokenissuancepolicy?view=graph-rest-beta) 资源类型，它控制由 Azure AD 颁发的 SAML 令牌的特征。 它允许你设置用于颁发 SAML 令牌的签名算法、签名选项或 SAML 令牌版本。
| 添加项 | beta | 新增了“[错误](/graph/api/resources/synchronization-synchronizationError?view=graph-rest-beta)”属性至**quarantineStatus** 资源类型。|
| 更改 | beta | 已使用请求程序、审批和审阅设置的附加属性更新了 [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)。|
| 添加项 | Beta 和 v1.0 | 添加了应用程序级和委派的 Policy.ReadWrite.ApplicationConfiguration 权限，以读取和写入有关应用程序配置策略的操作。|

### <a name="identity-and-access--information-protection"></a>身份和访问 | 信息保护

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 添加了 [create](/graph/api/informationprotection-post-threatassessmentrequests?view=graph-rest-1.0)、[get](/graph/api/threatassessmentrequest-get?view=graph-rest-1.0) 和 [list](/graph/api/informationprotection-list-threatassessmentrequests?view=graph-rest-1.0) API 以管理 [threatAssessmentRequest](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0) 资源。|

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | Beta | 已为租户中的所有频道邮件和租户中的所有聊天邮件添加[通知](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)。 |
| 添加项 | Beta | 新增了[swapShiftsChangeRequest: decline](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta) 方法至 **swapShiftsChangeRequest** 资源。 |

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | v1.0 | 添加了 [user: reprocessLicenseAssignment API](/graph/api/user-reprocesslicenseassignment)，它可用于重新处理[用户](/graph/api/resources/user?view=graph-rest-1.0)的所有基于组的许可证分配。 |

## <a name="january-2020"></a>2020 年 1 月

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version** | **说明** |
|:---|:---|:---|
|Addition|beta|添加的新实体：<br/>[androidDeviceOwnerImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[intune-device-comanagementEligibleDeviceEntity](/graph/api/resources/comanagementEligibleDeviceEntity?view=graph-rest-beta)<br/>[comanagementEligibleSummaryEntity](/graph/api/resources/intune-device-comanagementEligibleSummaryEntity?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[appleVpnAlwaysOnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnalwaysonconfiguration?view=graph-rest-beta)<br/>[deviceManagementIntentSettingSecretConstraint](/graph/api/resources/intune-deviceintent-devicemanagementintentsettingsecretconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingAppConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingappconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingCollectionConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingcollectionconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingEnrollmentTypeConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingenrollmenttypeconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingRequiredConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingrequiredconstraint?view=graph-rest-beta)<br/>[iosCredentialSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-ioscredentialsinglesignonextension?view=graph-rest-beta)<br/>[iosRedirectSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-iosredirectsinglesignonextension?view=graph-rest-beta)<br/>[iosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-iossinglesignonextension?view=graph-rest-beta)<br/>[macOSCredentialSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-macoscredentialsinglesignonextension?view=graph-rest-beta)<br/>[macOSRedirectSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-macosredirectsinglesignonextension?view=graph-rest-beta)<br/>[macOSSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-macossinglesignonextension?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationSettingState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationsettingstate?view=graph-rest-beta)<br/>[specifiedCaptiveNetworkPlugins](/graph/api/resources/intune-deviceconfig-specifiedcaptivenetworkplugins?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新枚举类型：<br/>[coManagementEligibleType](/graph/api/resources/intune-devices-comanagementeligibletype?view=graph-rest-beta)<br/>[vpnServiceExceptionAction](/graph/api/resources/intune-deviceconfig-vpnserviceexceptionaction?view=graph-rest-beta)<br/>[vpnTunnelConfigurationType](/graph/api/resources/intune-deviceconfig-vpntunnelconfigurationtype?view=graph-rest-beta)<br/>|
|添加项|beta|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) 上添加了 [wipeAndBlockManagedApps](/graph/api/api/intune-mam-user-wipeandblockmanagedapps?view=graph-rest-beta) 操作 |
|添加项|beta|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) 上添加了 [unblockManagedApps](/graph/api/intune-mam-user-unblockmanagedapps?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceShellScript](/graph/api/resources/intune-devices-deviceshellscript?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-devices-deviceshellscript-assign?view=graph-rest-beta) 操作 |
|添加项|beta|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) 集合上添加了 [getManagedAppBlockedUsers](/graph/api/intune-mam-user-getmanagedappblockedusers?view=graph-rest-beta) 函数 |
|添加项|beta|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) 上添加了 [isManagedAppUserBlocked](/graph/api/intune-mam-user-ismanagedappuserblocked?view=graph-rest-beta) 函数 |
|添加项|beta|向 [androidWorkProfileEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **proxySettings** 和 **proxyAutomaticConfigurationUrl** 属性|
|添加项|beta|向 [deviceManagementSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementsettingdefinition?view=graph-rest-beta) 实体添加了 **placeholderText** 属性|
|添加项|beta|向 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) 实体添加了 **iosSingleSignOnExtension** 属性|
|添加项|beta|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **kioskModeAppType** 属性|
|添加项|beta|向 [iosikEv2VpnConfiguration](/graph/api/resources/intune-deviceconfig-iosikev2vpnconfiguration?view=graph-rest-beta) 实体添加了 **alwaysOnConfiguration** 和 **enableAlwaysOnConfiguration** 属性|
|更改|beta|更改了 [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) 实体上的以下属性：<br/>将 **utcTimeOffsetInMinutes** 从必需更改为可选<br/>|
|添加项|beta|向 [macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta) 实体添加了 **macOSSingleSignOnExtension** 属性|
|添加项|beta|向 [managedDeviceMobileAppConfigurationState](/graph/api/resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState?view=graph-rest-beta) 实体添加了 **settingStates** 属性|
|添加项|beta|向 [deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-beta) 复杂类型添加了 **blockedManufacturers** 属性|
|添加项|beta|向 [iosKerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-ioskerberossinglesignonextension?view=graph-rest-beta) 复杂类型添加了 **realm**、**domains**、**blockAutomaticLogin**、**cacheName**、**credentialBundleIdAccessControlList**、**domainRealms**、**isDefaultRealm**、**passwordBlockModification**、**passwordExpirationDays**、**passwordExpirationNotificationDays**、**userPrincipalName**、**passwordRequireActiveDirectoryComplexity**、**passwordPreviousPasswordBlockCount**、**passwordMinimumLength**、**passwordMinimumAgeDays**、**passwordRequirementsDescription**、**requireUserPresence**、**activeDirectorySiteCode**、**passwordEnableLocalSync**、**blockActiveDirectorySiteAutoDiscovery** 和 **passwordChangeUrl** 属性|
|添加项|beta|向 [macOSKerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-macoskerberossinglesignonextension?view=graph-rest-beta) 复杂类型添加了 **realm**、**domains**、**blockAutomaticLogin**、**cacheName**、**credentialBundleIdAccessControlList**、**domainRealms**、**isDefaultRealm**、**passwordBlockModification**、**passwordExpirationDays**、**passwordExpirationNotificationDays**、**userPrincipalName**、**passwordRequireActiveDirectoryComplexity**、**passwordPreviousPasswordBlockCount**、**passwordMinimumLength**、**passwordMinimumAgeDays**、**passwordRequirementsDescription**、**requireUserPresence**、**activeDirectorySiteCode**、**passwordEnableLocalSync**、**blockActiveDirectorySiteAutoDiscovery** 和 **passwordChangeUrl** 属性|
|添加项|beta|向 [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **alwaysOn** 成员|
|添加项|beta|向 [deviceManagementTemplateType](/graph/api/resources/intune-deviceintent-devicemanagementtemplatetype?view=graph-rest-beta) 枚举类型添加了 **deviceCompliance** 成员|
|添加项|beta|向 [windowsAutopilotDeviceType](/graph/api/resources/intune-enrollment-windowsautopilotdevicetype?view=graph-rest-beta) 枚举类型添加了 **holoLens** 成员|

### <a name="identity-and-access"></a>身份和访问 

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
|更改 | beta |现有策略集将替换为[策略](/graph/api/resources/policy-overview?view=graph-rest-beta) URL 段。 键入的策略资源现在在“策略”段下分组，详见“[此博客文章](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/)”中的说明。 此更新添加 4 个类型的策略资源： <br> <li>[activityBasedTimeoutPolicies](/graph/api/resources/activityBasedTimeoutPolicy?view=graph-rest-beta)</li> <li>[claimsMappingPolicies](/graph/api/resources/claimsMappingPolicy?view=graph-rest-beta) </li> <li>[homeRealmDiscoveryPolicies](/graph/api/resources/homeRealmDiscoveryPolicy?view=graph-rest-beta) 和 </li> <li>[tokenLifetimePolicies](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta)</li> |
| Addition | beta | 对于支持基于活动的超时功能的应用程序，添加的 [activityBasedTimeoutPolicy](/graph/api/resources/activityBasedTimeoutPolicy?view=graph-rest-beta) 资源类型控制着一段时间不活动后 Web 会话的自动注销。|
| Addition | beta |[claimsMappingPolicy](/graph/api/resources/claimsMappingPolicy?view=graph-rest-beta) 资源类型控制用于 WS-AT、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射，适用于向特定应用程序发出的令牌。|
| Addition | beta | [homeRealmDiscoveryPolicy](/graph/api/resources/homeRealmDiscoveryPolicy?view=graph-rest-beta) 资源类型控制联盟用户的 Azure Active Directory 身份验证行为，尤其适用于联合域中的自动加速和用户身份验证限制。 |
| Addition | beta | [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta) 资源类型控制用于访问受保护资源的访问令牌的生存期持续时间。|
|添加项| beta| 向 [List provisioningObjectSummary](/graph/api/resources/provisioning-object-summary-list?view=graph-rest-beta) 添加了 servicePrincipal 属性。|

### <a name="security"></a>安全性

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改 | Beta 和 v1.0 | [更新警报](/graph/api/alert-update?view=graph-rest-1.0&tabs=http)方法现仅使用以下值更新**批注**字段： <br/> `Closed in IPC`, `Closed in MCAS`.|

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加 | v1.0 | 向团队资源类型添加了 **primaryChannel** 导航属性。|

### <a name="users"></a>用户

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | v1.0 | 向 [user](/graph/api/resources/user?view=graph-rest-1.0) 资源添加了 **identities** 属性。 此属性表示此用户可用于登录的标识集（如本地帐户和社交帐户）。|

## <a name="december-2019"></a>2019 年 12 月

### <a name="change-notifications"></a>更改通知

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 增加了对包含资源数据的通知订阅的支持。 目前支持的资源是 Microsoft Teams 频道和聊天中的 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 资源。 订阅应用必须实施其他授权和解密代码才能使用此功能。 有关详细信息，请参阅[设置聊天消息（包括消息属性）的更改通知（预览版）](webhooks-with-resource-data.md)。|

### <a name="cloud-communications"></a>云通信

在 beta 版中引入了状态并在 v1.0 中添加了云通信。

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
|Addition|beta|添加[状态](/graph/api/resources/presence?view=graph-rest-beta)资源和关联的方法，并引入了 Presence.Read 和 Presence.Read.All 权限。|
|添加|v1.0|添加了以下 API：[创建呼叫](/graph/api/application-post-calls?view=graph-rest-1.0)、[呼叫应答](/graph/api/call-answer?view=graph-rest-1.0)、[呼叫拒接](/graph/api/call-reject?view=graph-rest-1.0)、[呼叫获取](/graph/api/call-get?view=graph-rest-1.0)、[呼叫删除](/graph/api/call-delete?view=graph-rest-1.0)、[呼叫静音](/graph/api/call-mute?view=graph-rest-1.0)、[呼叫取消静音](/graph/api/call-unmute?view=graph-rest-1.0)、[呼叫更改屏幕共享角色](/graph/api/call-changescreensharingrole?view=graph-rest-1.0)、[呼叫转移](/graph/api/call-transfer?view=graph-rest-1.0)、[呼叫重定向](/graph/api/call-redirect?view=graph-rest-1.0)、[播放提示](/graph/api/call-playprompt?view=graph-rest-1.0)、[记录回复](/graph/api/call-recordresponse?view=graph-rest-1.0)、[订阅铃声](/graph/api/call-subscribetotone?view=graph-rest-1.0)、[列出参与者](/graph/api/call-list-participants?view=graph-rest-1.0)、[邀请参与者](/graph/api/participant-invite?view=graph-rest-1.0)、[获取参与者](/graph/api/participant-get?view=graph-rest-1.0)、[使参与者静音](/graph/api/participant-mute?view=graph-rest-1.0)、[创建联机会议](/graph/api/application-post-onlinemeeting?view=graph-rest-1.0)、[获取联机会议](/graph/api/onlinemeeting-get?view=graph-rest-1.0)以及[呼叫保持活动](/graph/api/call-keepalive?view=graph-rest-1.0)。|
|添加|v1.0|添加了以下资源： [call](/graph/api/resouces/call?view=graph-rest-1.0)、[参与者](/graph/api/resouces/participant?view=graph-rest-1.0)和[onlineMeeting](/graph/api/resouces/onlinemeeting?view=graph-rest-1.0)。|
| 更改        | Beta        | 已将 IVR API 记录重命名为 [recordResponse](/graph/api/call-record?view=graph-rest-beta)。 |
| 更改        | Beta        | 删除了 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta) 对象属性 **isCanceled**、**canceledDateTime** 和 **entryExitAnnouncement**。 已将属性 **joinUrl** 重命名为 **joinWebUrl**。 |
| 添加项        | Beta 和 v1.0       | 添加了 [delete onlineMeeting](/graph/api/onlinemeeting-delete.md) 操作。|

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
|Addition|beta|添加的新实体：<br/>[deviceShellScript](/graph/api/resources/intune-devices-deviceshellscript?view=graph-rest-beta)<br/>|
|添加|beta|新增了复杂类型：<br/>[deviceManagementSettingFileConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingfileconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingProfileConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingprofileconstraint?view=graph-rest-beta)<br/>[redirectSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-redirectsinglesignonextension?view=graph-rest-beta)<br/>[retireScheduledManagedDevice](/graph/api/resources/intune-deviceconfig-retirescheduledmanageddevice?view=graph-rest-beta)<br/>|
|添加|beta|添加的新枚举类型：<br/>[defenderRealtimeScanDirection](/graph/api/resources/intune-deviceconfig-defenderrealtimescandirection?view=graph-rest-beta)<br/>[managedAppDataIngestionLocation](/graph/api/resources/intune-mam-managedappdataingestionlocation?view=graph-rest-beta)<br/>[managedDeviceArchitecture](/graph/api/resources/intune-devices-manageddevicearchitecture?view=graph-rest-beta)<br/>[mdmSupportedState](/graph/api/resources/intune-gpanalyticsservice-mdmsupportedstate?view=graph-rest-beta)<br/>[scheduledRetireState](/graph/api/resources/intune-deviceconfig-scheduledretirestate?view=graph-rest-beta)<br/>|
|Addition|beta|在 [deviceCompliancePolicy](/graph/api/resources/intune-shared-devicecompliancepolicy?view=graph-rest-beta) 集合上添加了 [getDevicesScheduledToRetire](o:getDevicesScheduledToRetire:Collection(microsoft.graph.deviceCompliancePolicy)) 操作。 |
|Addition|beta|在 [deviceCompliancePolicy](/graph/api/resources/intune-shared-devicecompliancepolicy?view=graph-rest-beta) 集合上添加了 [setScheduledRetireState](o:setScheduledRetireState:Collection(microsoft.graph.deviceCompliancePolicy)) 操作 |
|Addition|beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 新增了 [wipe](/graph/api/intune-devices-manageddevice-wipe) 操作 |
|删除|beta|删除了 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上的[擦除](/graph/api/intune-devices-manageddevice-wipe)操作 |
|Addition|beta|向 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体添加了 **advancedThreatProtectionRequiredSecurityLevel** 和 **securityBlockDeviceAdministratorManagedDevices** 属性|
|Addition|beta|向 [androidDeviceOwnerCompliancePolicy](/graph/api/resources/intune-deviceconfig-androiddeviceownercompliancepolicy?view=graph-rest-beta) 实体添加了 **advancedThreatProtectionRequiredSecurityLevel** 属性|
|添加项|beta|向 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **certificateCredentialConfigurationDisabled** 属性|
|添加项|beta|向 [androidManagedAppProtection](/graph/api/resources/intune-shared-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **allowedAndroidDeviceModels** 和 **appActionIfAndroidDeviceModelNotAllowed** 属性|
|Addition|beta|向 [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) 实体添加了 **advancedThreatProtectionRequiredSecurityLevel** 属性|
|Addition|beta|向 [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta) 实体添加了 **subjectNameFormatString**、**certificateStore** 和 **customSubjectAlternativeNames** 属性|
|Addition|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了**allowedAndroidDeviceModels** 和 **appActionIfAndroidDeviceModelNotAllowed** 属性|
|添加|beta|向 [deviceHealthScriptRunSummary](/graph/api/resources/intune-devices-devicehealthscriptrunsummary?view=graph-rest-beta) 实体添加了 **issueRemediatedCumulativeDeviceCount** 属性|
|Addition|beta|向 [groupPolicySettingMapping](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingmapping?view=graph-rest-beta) 实体添加了 **mdmSupportedState** 属性|
|Addition|beta|向 [iosPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-iospkcscertificateprofile) 实体添加了 **subjectNameFormatString**, **certificateStore** 和 **customSubjectAlternativeNames** 属性|
|Addition|beta|向 [macOSMicrosoftEdgeApp](/graph/api/resources/intune-apps-macosmicrosoftedgeapp?view=graph-rest-beta)实体添加了 **频道**属性|
|添加项|beta|向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体添加了 **blockDataIngestionIntoOrganizationDocuments** 和 **allowedDataIngestionLocations** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **physicalMemoryInBytes** 和 **processorArchitecture** 属性|
|添加项|beta|向 [userExperienceAnalyticsDeviceStartupHistory](/graph/api/resources/intune-devices-userexperienceanalyticsdevicestartuphistory?view=graph-rest-beta) 实体添加了 **isFeatureUpdate** 和 **operatingSystemVersion** 属性|
|Addition|beta|将 **defenderDisableScanArchiveFiles**、**defenderDisableBehaviorMonitoring**、**defenderDisableCloudProtection**、**defenderEnableScanIncomingMail**、**defenderEnableScanMappedNetworkDrivesDuringFullScan**、**defenderDisableScanRemovableDrivesDuringFullScan**、**defenderDisableScanDownloads**、**defenderDisableIntrusionPreventionSystem**、**defenderDisableOnAccessProtection**、**defenderDisableRealTimeMonitoring**, **defenderDisableScanNetworkFiles**、**defenderDisableScanScriptsLoadedInInternetExplorer**、**defenderBlockEndUserAccess**, **defenderScanMaxCpuPercentage**、**defenderCheckForSignaturesBeforeRunningScan**、**defenderCloudBlockLevel**、**defenderCloudExtendedTimeoutInSeconds**、**defenderDaysBeforeDeletingQuarantinedMalware**、**defenderDisableCatchupFullScan**、**defenderDisableCatchupQuickScan**、 **defenderEnableLowCpuPriority**、**defenderFileExtensionsToExclude**、 **defenderFilesAndFoldersToExclude**、**defenderProcessesToExclude**、 **defenderPotentiallyUnwantedAppAction**、**defenderScanDirection**、 **defenderScanType**、**defenderScheduledQuickScanTime**、**defenderScheduledScanDay**、**defenderScheduledScanTime**、**defenderSubmitSamplesConsentType** 和 **defenderDetectedMalwareActions** 属性添加至 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了**uninstallBuiltInApps** 属性|
|添加|beta|向 [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) 实体增加了 **subjectNameFormatString**、**certificateStore** 和 **customSubjectAlternativeNames** 属性|
|添加|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceShellScripts** 导航属性|
|添加项|beta|向 [kerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-kerberossinglesignonextension?view=graph-rest-beta) 复杂类型添加了**passwordChangeUrl**属性|
|添加|beta|向 [groupPolicySettingType](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingtype?view=graph-rest-beta) 枚举类型添加了 **securityOptions**、**userRightsAssignment**、**auditSetting** 和 **windowsFirewallSettings**成员|
|Addition|beta|向 [resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta) 枚举类型添加了 **contentDownloaded** 成员|

### <a name="education"></a>教育

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | v1.0 | 已将 [classSettings](/graph/api/resources/teamclasssettings?view=graph-rest-1.0) 属性添加到[团队](/graph/api/resources/team?view=graph-rest-1.0)资源，以允许调用方获取特定于班级类型的团队的设置。|

### <a name="groups"></a>组

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition        | Beta          |向 [group](/graph/api/resources/group?view=graph-rest-1.0) 实体添加了 **hideFromAddressLists** 和 **hideFromOutlookClients** 属性，用于控制一个组在 Outlook UI 中的可见性。|

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
|更改 | beta |更新了 [servicePrincipal](/graph/api/resources/serviceprincipal.md) 中的 **appRoleAssignments** 和 **appRoleAssignedTo** 关系的行为以返回记录的角色。 **appRoleAssignments** 返回向服务主体授予的应用程序角色，而 **appRoleAssignedTo** 返回向服务主体授予应用程序角色的主体。|
| Addition | beta | 添加了新的实体类型 [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)。 |
|添加项|beta、v1.0|添加了以下支持：当应用程序无法访问响应集中的某些类型时，返回有限的信息。 有关更多详细信息，请参阅[为不可访问的成员对象返回有限的信息](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects)。|

### <a name="identity-and-access--information-protection"></a>身份和访问 | 信息保护

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | beta        | 添加了 [create](/graph/api/informationprotection-post-threatassessmentrequests?view=graph-rest-beta)、[get](/graph/api/threatassessmentrequest-get?view=graph-rest-beta) 和 [list](/graph/api/informationprotection-list-threatassessmentrequests?view=graph-rest-beta) API 以管理 [threatAssessmentRequest](/graph/api/resources/threatAssessmentRequest?view=graph-rest-beta) 资源。|
| 添加项        | beta        | 向 [evaluate application](/graph/api/informationprotectionlabel-evaluateapplication?view=graph-rest-beta)、[evaluate classification](/graph/api/informationprotectionlabel-evaluateclassificationresults?view=graph-rest-beta)、[evaluate removal](/graph/api/informationprotectionlabel-evaluateremoval?view=graph-rest-beta)、[extract label](/graph/api/informationprotectionlabel-extractlabel?view=graph-rest-beta)、[list label](/graph/api/informationprotectionlabel-list-labels?view=graph-rest-beta) 和 [get label](/graph/api/informationprotectionlabel-get?view=graph-rest-beta) 添加了可选请求标头 User-Agent。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包

介绍 Microsoft Graph 工具包的 1.1 版。

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项        | 不适用         | 新增 [mgt-get](/graph/toolkit/components/get) 组件。 |
| 添加项        | 不适用         | 新增了 [代理服务器提供商](/graph/toolkit/providers/proxy)。 |
| 添加项        | 不适用          | 向[人员卡组件](/graph/toolkit/components/person)添加了 `inherit-details` 属性。 |
| 添加项        | 不适用         | 向[人员选取器组件](/graph/toolkit/components/people-picker)添加了 `selectedPeople` 属性。 |
| 添加项        | 不适用        | 向[人员选取器组件](/graph/toolkit/components/people-picker)添加了 `loading` 和 `error` 模板。 |
| 添加项        | 不适用        | 向[任务组件](/graph/toolkit/components/tasks)添加了 `task` 和`task-details` 模板。 |
| 添加项        | 不适用          | 向[任务组件](/graph/toolkit/components/tasks)添加了 `isNewTaskVisible` 属性。 |
| 添加项        | 不适用        | 向[任务组件](/graph/toolkit/components/tasks)添加了 `group-id` 属性。 |
| 添加项        | 不适用          | 向[任务组件](/graph/toolkit/components/tasks)添加了 `taskFilter` 属性。 |
| 添加项        | 不适用         | 向[日程组件](/graph/toolkit/components/agenda)添加了 `eventClick` 事件。 |
| 添加项        | 不适用          | 向[人员组件](/graph/toolkit/components/people)添加了 `person-card` 属性。 |
| 添加项        | 不适用          | 向[人员组件](/graph/toolkit/components/people)添加了 `user-ids` 属性。 |
| 修补程序        | 不适用         | [Bug 修复和改进](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases/tag/v1.1.0)。 |

### <a name="people-and-workplace-intelligence--insights"></a>人脉和工作场所智能|见解

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | v1.0 | Insights API 现在提供  v1.0 版。 这包括[officeGraphInsights](/graph/api/resources/officegraphinsights?view=graph-rest-1.0)、[trending](/graph/api/resources/insights-trending?view=graph-rest-1.0)、[usedInsight](/graph/api/resources/insights-used?view=graph-rest-1.0)和 [sharedInsight](/graph/api/resources/insights-shared?view=graph-rest-1.0)资源，以及相关类型和方法。 查看[为什么与基于文档的见解集成？](social-intel-concept-overview.md#why-integrate-with-document-based-insights)了解更多信息。 |

### <a name="reports--office-365-usage-reports"></a>报告 | Office 365 使用率报告

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 更改          | Beta 和 v1.0  | 若要获得委派权限以允许应用代表用户读取 Office 365 服务使用情况报告，租户管理员必须事先为用户分配 Azure AD 受限管理员角色。 有关更多详细信息，请参阅[授权 API 读取 Office 365 使用情况报告](reportroot-authorization.md)。|

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 为新的和编辑过的频道消息和聊天消息添加了[通知](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)。 |
| 添加项 | Beta | 添加了 [shiftpreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta) 资源及相关方法。|
| 添加项 | Beta | 向 [userSettings](/graph/api/resources/usersettings?view=graph-rest-beta) 实体添加了新的关系 `shiftPreferences`。 |
| 更改 | Beta | 更新了执行班次资源（包括 [schedule](/graph/api/resources/schedule?view=graph-rest-beta)、[schedulingGroup](/graph/api/resources/schedulinggroup?view=graph-rest-beta)、[shift](/graph/api/resources/shift?view=graph-rest-beta)、[timeOff](/graph/api/resources/timeoff?view=graph-rest-beta)、[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta)、[timeOffRequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta)、[swapShiftChangeRequest](/graph/api/resources/swapshiftchangerequest?view=graph-rest-beta) 和 [openShiftChangeRequest](/graph/api/resources/openshiftchangerequest?view=graph-rest-beta)）读写操作所需的应用程序权限。 **注意：** 应用程序权限当前为个人预览版，不可用于公共用途。|

## <a name="november-2019"></a>2019 年 11 月

### <a name="calendar--place"></a>日历 | 位置

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | Beta  | 增加了[更新会议室或会议室列表](/graph/api/resources/place-get?view=graph-rest-beta)的能力。|

### <a name="cloud-communications--calls-and-online-meetings"></a>云通信 |呼叫和联机会议

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 更改        | Beta        | 已将[静音](/graph/api/call-mute?view=graph-rest-beta)和[参与者静音](/graph/api/participant-mute?view=graph-rest-beta)方法的返回类型从 [commsOperation](/graph/api/resources/commsoperation?view=graph-rest-beta) 更改为 [muteParticipantOperation](/graph/api/resources/muteparticipantoperation?view=graph-rest-beta)。 |
| 更改        | Beta        | 已将[取消静音](/graph/api/call-unmute?view=graph-rest-beta)方法的返回类型从 [commsOperation](/graph/api/resources/commsoperation?view=graph-rest-beta) 更改为 [unmuteParticipantOperation](/graph/api/resources/unmuteparticipantoperation?view=graph-rest-beta)。 |
| 添加        | Beta        | 向 [call](/api-reference/beta/resources/call.md) 实体添加了 [keepAlive](/api-reference/beta/api/call-keepalive.md) 操作。 |

### <a name="cloud-communications--recording"></a>云通信 | 录制

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加|beta|已将新操作 [updateRecordingStatus](/graph/api/call-updaterecordingstatus?view=graph-rest-beta) 添加至 [call](/graph/api/resources/call?view=graph-rest-beta) 实体。
|添加项|beta|添加了新的复杂类型 [incomingContext](/graph/api/resources/incomingcontext?view=graph-rest-beta)。
|添加项|beta|已将新属性 `incomingContext` 添加到 [call](/graph/api/resources/call?view=graph-rest-beta) 实体。
|添加项|beta|已将新属性 `endpointType` 添加到 [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-beta) 复杂类型。
|添加项|beta|已将新属性 `endpointType` 添加到 [invitationParticipantInfo](/graph/api/resources/invitationparticipantinfo?view=graph-rest-beta) 复杂类型。
|添加项|beta|已将新属性 `recordingStatus` 添加到 [recordingInfo](/graph/api/resources/recordinginfo?view=graph-rest-beta) 复杂类型。
|删除|beta|已从 [recordingInfo](/graph/api/resources/recordinginfo?view=graph-rest-beta) 复杂类型删除了属性 `status`。
|删除|beta|已从 [invitationParticipantInfo](/graph/api/resources/invitationparticipantinfo?view=graph-rest-beta) 复杂类型删除了f [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-beta)的继承。


### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version**   | **说明**                          |
|:---|:---|:---|
|添加|beta|添加的新实体：<br/>[complianceManagementPartner](/graph/api/resources/intune-onboarding-compliancemanagementpartner?view=graph-rest-beta)<br/>[macOSCustomAppConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomappconfiguration?view=graph-rest-beta)<br/>[macOSWiredNetworkConfiguration](/graph/api/resources/intune-deviceconfig-macoswirednetworkconfiguration?view=graph-rest-beta)<br/>|
|Addition|beta|新增了复杂类型：<br/>[companyPortalBlockedAction](/graph/api/resources/intune-shared-companyportalblockedaction?view=graph-rest-beta)<br/>[complianceManagementPartnerAssignment](/graph/api/resources/intune-onboarding-compliancemanagementpartnerassignment?view=graph-rest-beta)<br/>[deviceManagementPartnerAssignment](/graph/api/resources/intune-onboarding-devicemanagementpartnerassignment?view=graph-rest-beta)<br/>[roleScopeTagInfo](/graph/api/resources/intune-auditing-rolescopetaginfo?view=graph-rest-beta)<br/>[rotateBitLockerKeysDeviceActionResult](/graph/api/resources/intune-devices-rotatebitlockerkeysdeviceactionresult?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新枚举类型：<br/>[companyPortalAction](/graph/api/resources/intune-shared-companyportalaction?view=graph-rest-beta)<br/>[easServices](/graph/api/resources/intune-deviceconfig-easservices?view=graph-rest-beta)<br/>[managedBrowserType](/graph/api/resources/intune-mam-managedbrowsertype?view=graph-rest-beta)<br/>[wiredNetworkInterface](/graph/api/resources/intune-deviceconfig-wirednetworkinterface?view=graph-rest-beta)<br/>|
|添加项|beta|在 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 上添加了 [updateDeviceProperties](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties?view=graph-rest-beta) 操作 |
|添加项|beta|在 [groupPolicyConfiguration](/graph/api/resources/intune-grouppolicy-grouppolicyconfiguration?view=graph-rest-beta) 上添加了 [updateDefinitionValues](/graph/api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getPolicyNonComplianceMetadata](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata?view=graph-rest-beta) 操作 |
|删除|beta|删除了以下复杂类型：<br/>**scopeTagInfo**<br/>|
|删除|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上删除了 [getDeviceNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getdevicenoncompliancereports?view=graph-rest-beta) 操作 |
|删除|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上删除了 [getPolicyNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancereports?view=graph-rest-beta) 操作 |
|更改|beta|更改了 [androidDeviceOwnerCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androiddeviceownercertificateprofilebase?view=graph-rest-beta) 实体上的以下属性：<br/>将 **subjectAlternativeNameType** 从必需更改为可选<br/>|
|添加项|beta|将 **googleAccountsBlocked** 属性添加到 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体中|
|添加项|beta|将 **keyboardsRestricted** 和 **approvedKeyboards** 属性添加到 [androidManagedAppProtection](/graph/api/resources/intune-shared-androidmanagedappprotection?view=graph-rest-beta) 实体中|
|添加项|beta|将 **thirdPartyKeyboardsBlocked** 属性添加到 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体中|
|添加项|beta|将 **roleScopeTagIds** 属性添加到 [deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-beta) 实体中|
|删除|beta|从 [deviceManagementExportJob](/graph/api/resources/intune-reporting-devicemanagementexportjob?view=graph-rest-beta) 实体中删除 **orderBy** 属性|
|添加项|beta|将 **groupsRequiringPartnerEnrollment** 属性添加到 [deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta) 实体中|
|添加项|beta|将 **roleScopeTagIds** 属性添加到 [groupPolicyConfiguration](/graph/api/resources/intune-grouppolicy-grouppolicyconfiguration?view=graph-rest-beta) 实体中|
|添加项|beta|将 **companyPortalBlockedActions**、**showAzureADEnterpriseApps** 和 **showOfficeWebApps** 属性添加到 [intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta) 实体中|
|添加项|beta|将 **easServices** 和 **easServicesUserOverrideEnabled** 属性添加到 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体中|
|删除|beta|从 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **siriDisableServerLogging** 属性|
|添加项|beta|将 **thirdPartyKeyboardsBlocked** 属性添加到 [iosManagedAppProtection](/graph/api/resources/intune-shared-iosmanagedappprotection?view=graph-rest-beta) 实体中|
|添加项|beta|将 **managedBrowser** 属性添加到 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体中|
|添加项|beta|将 **ethernetMacAddress** 属性添加到 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体中|
|添加项|beta|将 **displayName** 属性添加到 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 实体中|
|添加项|beta|将 **managedDeviceCertificateStates** 导航属性添加到 [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta) 实体中|
|更改|beta|更改了 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 实体上的以下属性的类型：<br/>将 **assignments** 从 [deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta) 集合更改为[deviceHealthScriptAssignment](/graph/api/resources/intune-devices-devicehealthscriptassignment?view=graph-rest-beta) 集合<br/>|
|添加项|beta|将 **complianceManagementPartners** 导航属性添加到 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体中|
|添加项|beta|将 **userRoleScopeTags** 属性添加到 [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta) 复杂类型 |
|删除|beta|从 [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta) 复杂类型中删除 **scopeTags** 属性|
|更改|beta|更改了 [credentialSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-credentialsinglesignonextension?view=graph-rest-beta) 复杂类型上的以下属性：<br/>将 **teamIdentifier** 从必需更改为可选<br/>|
|添加项|beta|将 **companyPortalBlockedActions**、**showAzureADEnterpriseApps** 和 **showOfficeWebApps** 属性添加到 [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) 复杂类型|

### <a name="education"></a>教育

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta | 已将 [classSettings](/graph/api/resources/teamclasssettings?view=graph-rest-beta) 属性添加到[团队](/graph/api/resources/team?view=graph-rest-beta)资源，以允许调用方获取特定于班级类型的团队的设置。|

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 新增 | v1.0 | 添加了新实体类型：[应用程序](/graph/api/resources/application?view=graph-rest-1.0)。|
| 新增 | v1.0 | 添加了新委派权限 [Application.Read.All](/graph/permissions-reference#application-resource-permissions)、[Application.ReadWrite.All](/graph/permissions-reference#application-resource-permissions)。|
| 新增 | v1.0 | 添加了新的应用程序权限 [Application.Read.All](/graph/permissions-reference#application-resource-permissions)。|
| Addition | v1.0 | 添加了新的委派和应用程序权限[GroupMember](permissions-reference.md#group-permissions)和[GroupMember](permissions-reference.md#group-permissions) ，以获取和更新[组](/graph/api/resources/group?view=graph-rest-1.0)资源。
| 新增 | v1.0 | 添加了新的应用程序权限[组。创建](permissions-reference.md#group-permissions)以创建**组**资源。
| 添加项 | Beta 和 v1.0 | 向[用户](/graph/api/resources/user?view=graph-rest-1.0)资源添加了 **creationType** 属性。|
| 添加 | v1.0 | 添加了[设备](/graph/api/resources/device?view=graph-rest-1.0)资源的 [checkMemberObjects](/graph/api/device-checkmemberobjects?view=graph-rest-1.0) 操作。 |
| 新增 | v1.0 | 添加了[组](/graph/api/resources/group?view=graph-rest-1.0)资源的 [checkMemberObjects](/graph/api/group-checkmemberobjects?view=graph-rest-1.0) 操作。 |
| 添加 | v1.0 | 添加了[用户](/graph/api/resources/user?view=graph-rest-1.0)资源的 [checkMemberObjects](/graph/api/user-checkmemberobjects?view=graph-rest-1.0) 操作。 |

### <a name="identity-and-access--conditional-access"></a>身份和访问 | 条件访问

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加项 | beta | 增加了条件访问策略和命名位置中读取操作的 application-level Policy.Read.All 权限。|
| 添加项 | beta | 增加了对“仅报告”状态的支持：`enabledForReportingButNotEnforced`。|
| 更改 | beta | 更新了对条件访问策略和命名位置执行写操作所需的权限。|

### <a name="identity-and-access--information-protection"></a>身份和访问 | 信息保护

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | beta        | 向读取和写入威胁评估请求添加了新的委托和应用程序权限 [ThreatAssessment.ReadWrite.All](permissions-reference.md#threat-assessment-permissions) 和 [ThreatAssessment.Read.All](permissions-reference.md#threat-assessment-permissions) |

### <a name="mail"></a>邮件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 新增 | v1.0 | 已将 **conversationIndex** 属性添加到 [message](/graph/api/resources/message?view=graph-rest-1.0) 及其派生类型 [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-v1.0)。|
| 添加项 | Beta | 增加了对 [Mail.ReadBasic](/graph/permissions-reference#mail-permissions) 委派权限和 [Mail.ReadBasic.All](/graph/permissions-reference#mail-permissions) 应用程序权限的支持，可[创建](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)、[获取](/graph/api/subscription-get?view=graph-rest-beta)、[更新](/graph/api/subscription-update?view=graph-rest-beta)和[删除](/graph/api/subscription-delete?view=graph-rest-beta)邮件更改通知的订阅。 |
| 添加 | v1.0 | 增加了对 Mail.ReadBasic 代理权限和 Mail.ReadBasic.All 应用程序的支持，可以：<br />- [列出邮件](/graph/api/user-list-messages?view=graph-rest-1.0)<br />- [获取邮件](/graph/api/message-get?view=graph-rest-1.0) <br />- [列出邮件文件夹](/graph/api/user-list-mailfolders?view=graph-rest-1.0)<br />- [获取邮件文件夹](/graph/api/mailfolder-get?view=graph-rest-1.0)<br />- [列出子文件夹](/graph/api/mailfolder-list-childfolders?view=graph-rest-1.0)<br />- [列出文件夹中的邮件](/graph/api/mailfolder-list-childfolders?view=graph-rest-1.0)<br />- [获取邮件 Delta](/graph/api/message-delta?view=graph-rest-1.0)<br />- [获取邮件文件夹 Delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) <br />- [创建](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)、[获取](/graph/api/subscription-get?view=graph-rest-1.0)、[更新](/graph/api/subscription-update?view=graph-rest-1.0)和[删除](/graph/api/subscription-delete?view=graph-rest-1.0)邮件更改通知订阅|


### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加项 | Beta | 添加了[配置文件 API](/graph/api/resources/profile?view=graph-rest-beta) 和关联的方法。 |

### <a name="search"></a>搜索

Microsoft 搜索现在公开了在 Microsoft Graph 中搜索和索引数据的方式。

| **更改类型** | **Version** | **说明**                              |
|:----------------|:------------|:---------------------------------------------|
| 添加项        | beta        | 添加了构成[查询](/graph/api/search-query?view=graph-rest-beta)和[索引](/graph/api/resource/indexing-api-overview?view=graph-rest-beta)功能的[Microsoft 搜索 API](search-concept-overview.md)。 |
| 添加项        | beta        | 添加了[查询](/graph/api/search-query?view=graph-rest-beta)操作。 |
| 添加项        | beta        | 添加了 [searchRequest](/graph/api/resources/searchrequest?view=graph-rest-beta)、[searchQuery](/graph/api/resources/searchquery?view=graph-rest-beta)、[searchQueryString](/graph/api/resources/searchquerystring?view=graph-rest-beta)、[searchResponse](/graph/api/resources/searchresponse?view=graph-rest-beta)、[searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) 和 [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) 复杂类型。 |
| 添加项        | beta        | 添加了 [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta)、[schema](/graph/api/resources/schema?view=graph-rest-beta)[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 和 [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) 实体以及这些实体公开的方法。 |

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | Beta | 增加了 [openshift](/graph/api/resources/openshift?view=graph-rest-beta)、[openshiftChangeRequest](/graph/api/resources/openshiftChangeRequest?view=graph-rest-beta)、[swapShiftChangeRequest](/graph/api/resources/swapShiftChangeRequest?view=graph-rest-beta)，以及 [timeoffrequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta) 资源和关联的方法。|
| 添加项 | Beta | 添加了 **timeClockEnabled**、**openShiftsEnabled**、**swapShiftsRequestsEnabled**、**offerShiftRequestsEnabled**、 **timeOffRequestsEnabled** 属性至 [日程安排](/graph/api/resources/schedule?view=graph-rest-beta)资源。|
| 添加项        | Beta          | 添加了其他路由以使用团队和频道 ID [get driveItem](/graph/api/driveitem-get?view=graph-rest-beta) 检索 [driveItem]。 |

### <a name="october-2019"></a>2019 年 10 月

### <a name="calendar"></a>日历

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | Beta | 向 [event](/graph/api/resources/event?view=graph-rest-beta) 和 [eventMessageRequest](/graph/api/resources/eventmessagerequest?view=graph-rest-beta) 实体添加了 **allowNewTimeProposals** 属性。 |
| 添加项 | Beta | 将 **proposedNewTime** 可选参数添加到 **event** 的 [tentativelyAccept](/graph/api/event-tentativelyaccept?view=graph-rest-beta) 和 [decline](/graph/api/event-decline?view=graph-rest-beta) 方法中。 |
| 添加项 | Beta | 添加了基于 [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta) 的 [eventMessageResponse](/graph/api/resources/eventmessageresponse?view=graph-rest-beta) 实体，此外，还包括 **proposedNewTime** 和 **responseType** 属性。 |
| 添加项 | Beta | 向 [attendee](/graph/api/resources/attendee?view=graph-rest-beta) 复杂类型添加了 **proposedNewTime** 属性。 |

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加项 | Beta 和 v1.0 | 向 [group](/graph/api/resources/group?view=graph-rest-1.0) 资源添加了 **securityIdentifier** 属性。 |
| 添加项 | Beta 和 v1.0 | 向 [device](/graph/api/resources/group?view=graph-rest-1.0) 资源添加了 **mdmAppId** 属性。 |
| 添加项 | Beta | 已将 **manufacturer** 和 **model** 属性添加到 [device](/graph/api/resources/device?view=graph-rest-beta) 实体。 |
| 新增 | v1.0 | 添加了新实体 [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-v1.0)。 |
| 新增 | v1.0 | 添加了新的复杂类型 [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-v1.0)。 |
| Addition | v1.0 | 在 [organization](/graph/api/resources/organization?view=graph-rest-v1.0) 资源上为 **certificateBasedAuthConfiguration** 添加了新的关系。 这将支持 [Azure Active Directory 中基于证书的身份验证](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)。|
|添加项 | Beta | 添加了新实体 [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-beta)。 |
|添加项 | Beta | 添加了[获取](/graph/api/calendarpermission-get?view=graph-rest-beta)、[更新](/graph/api/calendarpermission-update?view=graph-rest-beta)和[删除](/graph/api/calendarpermission-delete?view=graph-rest-beta) API 来管理[日历](/graph/api/resources/calendar?view=graph-rest-beta)上的 [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-beta) 资源。 |
|添加项 | Beta | 添加了新的复杂类型 [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo?view=graph-rest-beta)。 |
| 添加项 | Beta | 向 [event](/graph/api/resources/event?view=graph-rest-beta) 实体添加了“isOnlineMeeting”****、“onlineMeetingProvider”**** 和“onlineMeeting”**** 属性。 “isOnlineMeeting”**** 和“onlineMeetingProvider”**** 是事件**** 的[创建](/graph/api/user-post-events?view=graph-rest-beta)和[更新](/graph/api/event-update?view=graph-rest-beta)方法。 |
| 添加项 | Beta | 向 [calendar](/graph/api/resources/calendar?view=graph-rest-beta) 实体添加了“defaultOnlineMeetingProviders”**** 和“allowedOnlineMeetingProviders”**** 属性。 |
| Addition | Beta | 向 [calendar](/graph/api/resources/calendar?view=graph-rest-beta) 实体添加了“isTallyingResponses”**** 属性。 |
| 添加项 | Beta | 向 [calendar](/graph/api/resources/calendar?view=graph-rest-beta) 实体添加了“isRemovable”**** 属性。 |
| 添加 | Beta | 向 [mailboxSettings](/graph/api/resources/mailboxSettings?view=graph-rest-beta) 实体添加了“delegateMeetingMessageDeliveryOptions”**** 属性。 |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|添加的新实体：<br/>[deviceHealthScriptAssignment](/graph/api/resources/intune-devices-devicehealthscriptassignment?view=graph-rest-beta)<br/>[deviceHealthScriptDeviceState](/graph/api/resources/intune-devices-devicehealthscriptdevicestate?view=graph-rest-beta)<br/>[deviceHealthScriptRunSummary](/graph/api/resources/intune-devices-devicehealthscriptrunsummary?view=graph-rest-beta)<br/>[deviceManagementCachedReportConfiguration](/graph/api/resources/intune-reporting-devicemanagementcachedreportconfiguration?view=graph-rest-beta)<br/>[deviceManagementExportJob](/graph/api/resources/intune-reporting-devicemanagementexportjob?view=graph-rest-beta)<br/>[deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta)<br/>[deviceManagementReportSchedule](/graph/api/resources/intune-reporting-devicemanagementreportschedule?view=graph-rest-beta)<br/>[groupPolicyMigrationReport](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreport?view=graph-rest-beta)<br/>[groupPolicySettingMapping](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingmapping?view=graph-rest-beta)<br/>[macOSMicrosoftEdgeApp](/graph/api/resources/intune-apps-macosmicrosoftedgeapp?view=graph-rest-beta)<br/>[macOSPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-macospkcscertificateprofile?view=graph-rest-beta)<br/>[userExperienceAnalyticsDevicePerformance](/graph/api/resources/intune-devices-userexperienceanalyticsdeviceperformance?view=graph-rest-beta)<br/>[userExperienceAnalyticsDeviceStartupHistory](/graph/api/resources/intune-devices-userexperienceanalyticsdevicestartuphistory?view=graph-rest-beta)<br/>[userExperienceAnalyticsRegressionSummary](/graph/api/resources/intune-devices-userexperienceanalyticsregressionsummary?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicy](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyAssignment](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary?view=graph-rest-beta)<br/>[windowsMicrosoftEdgeApp](/graph/api/resources/intune-apps-windowsmicrosoftedgeapp?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[androidDeviceOwnerGlobalProxy](/graph/api/resources/intune-deviceconfig-androiddeviceownerglobalproxy?view=graph-rest-beta)<br/>[androidDeviceOwnerGlobalProxyAutoConfig](/graph/api/resources/intune-deviceconfig-androiddeviceownerglobalproxyautoconfig?view=graph-rest-beta)<br/>[androidDeviceOwnerGlobalProxyDirect](/graph/api/resources/intune-deviceconfig-androiddeviceownerglobalproxydirect?view=graph-rest-beta)<br/>[groupPolicyObjectFile](/graph/api/resources/intune-gpanalyticsservice-grouppolicyobjectfile?view=graph-rest-beta)<br/>[mobileAppInstallTimeSettings](/graph/api/resources/intune-shared-mobileappinstalltimesettings?view=graph-rest-beta)<br/>[scopeTagInfo](/graph/api/resources/intune-auditing-scopetaginfo?view=graph-rest-beta)<br/>[win32LobAppRestartSettings](/graph/api/resources/intune-shared-win32lobapprestartsettings?view=graph-rest-beta)<br/>|
|添加项|beta 版本|添加的新枚举类型：<br/>[deviceManagementReportFileFormat](/graph/api/resources/intune-reporting-devicemanagementreportfileformat?view=graph-rest-beta)<br/>[deviceManagementReportStatus](/graph/api/resources/intune-reporting-devicemanagementreportstatus?view=graph-rest-beta)<br/>[deviceManagementScheduledReportRecurrence](/graph/api/resources/intune-reporting-devicemanagementscheduledreportrecurrence?view=graph-rest-beta)<br/>[diskType](/graph/api/resources/intune-devices-disktype?view=graph-rest-beta)<br/>[groupPolicyMigrationReadiness](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreadiness?view=graph-rest-beta)<br/>[groupPolicySettingScope](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingscope?view=graph-rest-beta)<br/>[groupPolicySettingType](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingtype?view=graph-rest-beta)<br/>[managedAppDeviceThreatLevel](/graph/api/resources/intune-mam-managedappdevicethreatlevel?view=graph-rest-beta)<br/>[microsoftEdgeChannel](/graph/api/resources/intune-apps-microsoftedgechannel?view=graph-rest-beta)<br/>[remediationState](/graph/api/resources/intune-devices-remediationstate?view=graph-rest-beta)<br/>[userExperienceAnalyticsSummarizedBy](/graph/api/resources/intune-devices-userexperienceanalyticssummarizedby?view=graph-rest-beta)<br/>[win32LobAppRestartBehavior](/graph/api/resources/intune-apps-win32lobapprestartbehavior?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyStatuses](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses?view=graph-rest-beta)<br/>|
|添加项|beta|在 [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) 上添加了 [approveApps](/graph/api/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-approveapps?view=graph-rest-beta) 操作 |
|添加项|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 集合上添加了 [executeAction](/graph/api/api/intune-devices-manageddevice-executeaction?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-devices-devicehealthscript-assign?view=graph-rest-beta) 操作 |
|添加项|beta|在 [groupPolicyMigrationReport](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreport?view=graph-rest-beta) 集合上添加了 [createMigrationReport](/graph/api/intune-gpanalyticsservice-grouppolicymigrationreport-createmigrationreport?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getDeviceNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getdevicenoncompliancereports?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getPolicyNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancereports?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getDeviceNonComplianceReport](/graph/api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getPolicyNonComplianceReport](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports ](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta)上添加了 [getHistoricalReport](/graph/api/intune-reporting-devicemanagementreports-gethistoricalreport?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) 上添加了 [getCachedReport](/graph/api/intune-reporting-devicemanagementreports-getcachedreport?view=graph-rest-beta) 操作 |
|添加项|beta|在 [windowsDefenderApplicationControlSupplementalPolicy](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-assign?view=graph-rest-beta) 操作 |
|添加项|beta|在 [userExperienceAnalyticsDevicePerformance](/graph/api/resources/intune-devices-userexperienceanalyticsdeviceperformance?view=graph-rest-beta) 上添加了 [summarizeDevicePerformanceDevices](/graph/api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices?view=graph-rest-beta) 函数 |
|添加项|beta|在 [userExperienceAnalyticsRegressionSummary](/graph/api/resources/intune-devices-userexperienceanalyticsregressionsummary?view=graph-rest-beta) 上添加了 [summarizeDeviceRegressionPerformance](/graph/api/intune-devices-userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance?view=graph-rest-beta) 函数 |
|删除|beta|删除了以下复杂类型：<br/>**deviceHealthScriptComplianceRule**<br/>|
|删除|beta|删除了以下枚举类型：<br/>**deviceHealthScriptComplianceRuleOperator**<br/>**deviceHealthScriptDetectionType**<br/>|
|删除|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 集合上删除了 [executeAction](/graph/api/intune-devices-manageddevice-executeaction?view=graph-rest-beta) 操作 |
|添加项|beta|向 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **globalProxy** 属性|
|添加项|beta|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBlockPersonalAppInstallsFromUnknownSources** 属性|
|添加项|beta|向 [androidManagedAppProtection](/graph/api/resources/intune-shared-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **minimumRequiredCompanyPortalVersion**、**minimumWarningCompanyPortalVersion** 和 **minimumWipeCompanyPortalVersion** 属性|
|添加项|beta|向 [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBlockPersonalAppInstallsFromUnknownSources** 属性|
|添加项|beta|向 [appVulnerabilityTask](/graph/api/resources/intune-partnerintegration-appvulnerabilitytask?view=graph-rest-beta) 实体添加了 **remediation** 属性|
|添加项|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **minimumRequiredCompanyPortalVersion**、**minimumWarningCompanyPortalVersion** 和 **minimumWipeCompanyPortalVersion** 属性|
|添加项|beta|向 [depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta) 实体添加了 **configurationWebUrl** 属性|
|添加项|beta|向 [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta) 实体添加了 **source** 和 **sourceId** 属性|
|添加项|beta|向 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 实体添加了 **publisher**、**version**、**displayName**、**description**、**detectionScriptContent**、**createdDateTime**、**lastModifiedDateTime**、**runAsAccount**、**enforceSignatureCheck**、**runAs32Bit** 和 **roleScopeTagIds** 属性|
|删除|beta|从 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 实体中删除了 **complianceRule** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-gpanalyticsservice-devicemanagement?view=graph-rest-beta) 实体添加了 **groupPolicyObjectFiles** 属性|
|删除|beta|从 [deviceManagementScript](/graph/api/resources/intune-shared-devicemanagementscript?view=graph-rest-beta) 实体中删除了 **runSchedule** 属性|
|删除|beta|从 [deviceManagementScriptDeviceState](/graph/api/resources/intune-devices-devicemanagementscriptdevicestate?view=graph-rest-beta) 实体中删除了 **lastSyncDateTime**、**preRemediationDetectionScriptOutput**、**remediationScriptError** 和 **postRemediationDetectionScriptOutput** 属性|
|删除|beta|从 [deviceManagementScriptRunSummary](/graph/api/resources/intune-devices-devicemanagementscriptrunsummary?view=graph-rest-beta) 实体中删除了 **compliantDeviceCount**、**notCompliantDeviceCount** 和 **pendingDeviceCount** 属性|
|添加项|beta|向 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 实体添加了 **platformType** 属性|
|添加项|beta|向 [enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta) 实体添加了 **source** 和 **sourceId** 属性|
|添加项|beta|向 [group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了 **mdmAppId** 和 **securityIdentifier** 属性|
|添加项|beta|向 [importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta) 实体添加了 **isDeleted** 属性|
|添加项|beta|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **filesNetworkDriveAccessBlocked**、**filesUsbDriveAccessBlocked** 和 **wifiPowerOnForced** 属性|
|删除|beta|从 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **wiFiBlockPowerModification** 属性|
|添加项|beta|向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体添加了 **previousPinBlockCount**、**maximumAllowedDeviceThreatLevel** 和 **mobileThreatDefenseRemediationAction** 属性|
|添加项|beta|向 [mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta) 实体添加了 **source** 和 **sourceId** 属性|
|添加|beta|向 [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta) 实体添加了 **androidMobileApplicationManagementEnabled** 和 **iosMobileApplicationManagementEnabled** 属性|
|更改|beta|更改了 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体上的以下属性：<br/>将 **energySaverOnBatteryThresholdPercentage** 从必需属性更改为可选属性<br/>将 **energySaverPluggedInThresholdPercentage** 从必需属性更改为可选属性<br/>|
|添加项|beta|向 [windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta) 实体添加了 **source** 和 **sourceId** 属性|
|添加项|beta|向 [channel](/graph/api/resources/channel?view=graph-rest-beta) 实体添加了 **filesFolder** 导航属性|
|添加项|beta|向 [deviceAppManagement](/graph/api/resources/intune-unlock-deviceappmanagement?view=graph-rest-beta) 实体添加了 **wdacSupplementalPolicies** 导航属性|
|添加项|beta|向 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) 实体添加了 **assignments**、**runSummary** 和 **deviceRunStates** 导航属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-devices-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceHealthScripts**、**userExperienceAnalyticsDevicePerformance**、**userExperienceAnalyticsRegressionSummary**、**userExperienceAnalyticsDeviceStartupHistory**、**groupPolicyMigrationReports** 和 **reports** 导航属性|
|添加项|beta|向 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) 实体添加了 **singleSignOnExtensionPkinitCertificate** 导航属性|
|添加项|beta|向 [macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta) 实体添加了 **singleSignOnExtensionPkinitCertificate** 导航属性|
|添加项|beta|向 [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta) 复杂类型添加了 **scopeTags** 属性|
|添加项|beta|向 [deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-beta) 复杂类型添加了 **androidDedicatedCount**、**androidDeviceAdminCount**、**androidFullyManagedCount** 和 **androidWorkProfileCount** 属性|
|添加项|beta|向 [win32LobAppAssignmentSettings](/graph/api/resources/intune-shared-win32lobappassignmentsettings?view=graph-rest-beta) 复杂类型添加了 **restartSettings** 和 **installTimeSettings** 属性|
|添加项|beta|向 [win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta) 复杂类型添加了 **deviceRestartBehavior** 属性|
|添加项|beta|向 [androidDeviceOwnerRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype?view=graph-rest-beta) 枚举类型添加了 **customPassword** 成员|
|删除|beta|从 [deviceEnrollmentType](/graph/api/resources/intune-shared-deviceenrollmenttype?view=graph-rest-beta) 枚举类型中删除了 **appleUserEnrollmentWithAzureAD** 成员|
|添加项|beta|向 [deviceManagementTemplateType](/graph/api/resources/intune-deviceintent-devicemanagementtemplatetype?view=graph-rest-beta) 枚举类型添加了 **microsoftEdgeSecurityBaseline** 和 **microsoftOffice365ProPlusSecurityBaseline** 成员|
|添加项|beta|向 [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta) 枚举类型添加了 **setDeviceName** 成员|
|添加项|beta|向 [runState](/graph/api/resources/intune-shared-runstate?view=graph-rest-beta) 枚举类型添加了 **scriptError** 和 **notApplicable** 成员|
|删除|beta|从 [runState](/graph/api/resources/intune-shared-runstate?view=graph-rest-beta) 枚举类型中删除了 **error** 成员|
|添加项|beta|向 [windowsHealthMonitoringScope](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringscope?view=graph-rest-beta) 枚举类型添加了 **userExperienceAnalytics** 成员|

### <a name="education"></a>教育

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 删除项 | beta | 已从 [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) 删除[以前公布的](https://developer.microsoft.com/onenote/blogs/breaking-change-education-api-updates-in-microsoft-graph-beta)已弃用的属性 **grade** 和 **feedback**。 仅通过 [educationOutcome](/graph/api/educationsubmission-list-outcomes?view=graph-rest-beta) 访问成绩和反馈。|

### <a name="groups"></a>组

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition        | Beta 版本          |向 [group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了 **hideFromAddressLists** 和 **hideFromOutlookClients** 属性，用于控制一个组在 Outlook 用户界面中的可见性。|
| 添加项 | Beta 版本 | 添加了 [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta) 方法，该方法可用于在 [group](/graph/api/resources/group?view=graph-rest-beta) 中的用户上添加或删除许可证。 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| Addition | Beta 版本 | 添加的新实体： <br/>[authenticationDetail](/graph/api/resources/authenticationDetail?view=graph-rest-beta)<br/>[keyValue](/graph/api/resources/keyValue?view=graph-rest-beta)<br/>[networkLocationDetail](/graph/api/resources/networkLocationDetail?view=graph-rest-beta)|
| 添加项 | Beta 版本 | 向 [signIn](/graph/api/resources/signin?view=graph-rest-beta) 资源添加了“alternateSignInName”****、“ServicePrincipalId”****、“ServicePrincipalName”**** 和“authenticationProcessingDetails”**** 属性。 |
| 删除 | Beta | 已将 [mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta) 的引用从 [signIn](/graph/api/resources/signin?view=graph-rest-beta) 移动到 [authenticationDetail](/graph/api/resources/authenticationDetail?view=graph-rest-beta)。 |
| 添加项 | Beta 版本 | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 资源添加了“signInActivity”**** 属性。 |
| 添加 | Beta 版本 | 添加了新实体类型：[Trustframeworkkeyset](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta) |
| 添加项 | Beta | 添加了新实体类型：[Identityuserflow](/graph/api/resources/identityuserflow?view=graph-rest-beta) |
| 添加项 | Beta | 添加了新的 [entitlement management](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) 资源。 |
| Addition | Beta | 向 [application](/graph/resources/application?view=graph-rest-beta) 资源添加了 [removePassword](/graph/api/application-removepassword?view=graph-rest-beta) 方法。 |
| Addition | Beta | 向 [application](/graph/resources/application?view=graph-rest-beta) 添加了“addIns”**** 属性。 |
| Addition | Beta | 向 [serviceprincipal](/graph/resources/serviceprincipal?view=graph-rest-beta) 资源添加了 [addPassword](/graph/api/serviceprincipal-addpassword?view=graph-rest-beta) 和 [removePassword](/graph/api/serviceprincipal-removepassword?view=graph-rest-beta) 方法。 |
| 添加项 | Beta 和 v1.0 | 向 [group](/graph/api/resources/group?view=graph-rest-1.0) 实体添加了“onPremisesDomainName”****、“onPremisesNetBiosName”**** 和“onPremisesSamAccountName”**** 属性。 |
| 添加项 | Beta 和 v1.0 | 向 [group](/graph/api/resources/group?view=graph-rest-1.0) 资源添加了 **securityIdentifier** 属性。 |
| 添加项 | Beta 和 v1.0 | 向 [device](/graph/api/resources/group?view=graph-rest-1.0) 资源添加了 **mdmAppId** 属性。 |
| 添加项 | Beta 和 v1.0 | 已将 **manufacturer** 和 **model** 属性添加到 [device](/graph/api/resources/device?view=graph-rest-1.0) 实体。 |
| 新增 | v1.0 | 添加了新的 [orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0) 资源。 这些联系人由组织管理，不同于[个人联系人](outlook-contacts-concept-overview.md)|
| 新增 | v1.0 | 添加了新的 [physicalOfficeAddress](/graph/api/resources/physicalOfficeAddress?view=graph-rest-1.0) 资源。 |
| 新增 | v1.0 | 添加了新实体 [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-1.0)。 |
| 新增 | v1.0 | 添加了新的复杂类型 [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-1.0)。 |
| Addition | v1.0 | 在 [organization](/graph/api/resources/organization?view=graph-rest-1.0) 资源上为 **certificateBasedAuthConfiguration** 添加了新的关系。 这将支持 [Azure Active Directory 中基于证书的身份验证](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)。|

### <a name="identity-and-access--conditional-access"></a>身份和访问 | 条件访问

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| Addition | Beta | 添加了新实体类型：<br/>[conditionalAccessPolicy](/graph/api/resources/conditionalAccessPolicy)<br/>
| Addition | Beta | 新增了复杂类型：<br/>[conditionalAccessSessionControl](/graph/api/resources/conditionalAccessSessionControl)<br/>[applicationEnforcedRestrictionsSessionControl](/graph/api/resources/applicationEnforcedRestrictionsSessionControl)<br/>[cloudAppSecuritySessionControl](/graph/api/resources/cloudAppSecuritySessionControl)<br/>[signInFrequencySessionControl](/graph/api/resources/signInFrequencySessionControl)<br/>[persistentBrowserSessionControl](/graph/api/resources/persistentBrowserSessionControl)<br/>[conditionalAccessSessionControls](/graph/api/resources/conditionalAccessSessionControls)<br/>[conditionalAccessApplications](/graph/api/resources/conditionalAccessApplications)<br/>[conditionalAccessUsers](/graph/api/resources/conditionalAccessUsers)<br/>[conditionalAccessPlatforms](/graph/api/resources/conditionalAccessPlatforms)<br/>[conditionalAccessLocations](/graph/api/resources/conditionalAccessLocations)<br/>[conditionalAccessDeviceStates](/graph/api/resources/conditionalAccessDeviceStates)<br/>[conditionalAccessConditionSet](/graph/api/resources/conditionalAccessConditionSet)<br/>[conditionalAccessGrantControls](/graph/api/resources/conditionalAccessGrantControls)<br/>|
| Addition | Beta | 添加了 [namedLocation API](/graph/api/resources/namedLocation?view=graph-rest-beta)，这表示 Azure AD 条件访问中的已命名位置。 |

### <a name="identity-and-access--information-protection"></a>身份和访问 | 信息保护

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改          | beta          | 已将 **detectedSensitiveContent** 实体名称更改为 [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta)。  |
| 删除        | beta          | 已从 [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta) 删除“displayName”****、“uniqueCount”**** 和“matches”**** 属性。  |
| 更改          | beta          | 已将“ID”**** 更改为 [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta) 的“sensitiveTypeId”**** 属性。   |
| 更改          | beta          | 已将“confidence”**** 更改为 [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta) 的“confidenceLevel”**** 属性。   |
| Addition        | beta          | 向 [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta)/ 添加了“count”**** 属性。  |
| 删除        | beta          | 从 [labelingOptions](/graph/api/resources/labelingoptions?view=graph-rest-beta) 删除了“actionSource”**** 属性。 |
| 删除        | beta          | 删除了“auditInfo”**** 实体。 |
| 更改          | beta          | 已将“protectByDoNotForwardAction”**** 更改为 [protectDoNotForwardAction](/graph/api/resources/protectdonotforwardaction?view=graph-rest-beta)。 |
| 添加        | beta          | 向 [addContentHeaderAction](/graph/api/resources/addcontentheaderaction?view=graph-rest-beta) 添加了“alignment”**** 属性。 |
| 更改          | beta          | 已将“labelId”**** 属性更改为 [recommendLabelAction](/graph/api/resources/recommendedlabelaction?view=graph-rest-beta) 中的“label”****。 |
| 更改          | beta          | 已将“classificationIds”**** 属性更改为 [recommendLabelAction](/graph/api/resources/recommendedlabelaction?view=graph-rest-beta) 中的“responsibleSensitivityTypeIds”****。 |
| Addition        | beta          | 向 [recommendLabelAction](/graph/api/resources/recommendedlabelaction?view=graph-rest-beta) 添加了“actionSource”**** 属性。 |
| 更改          | beta          | 已将“labelId”**** 属性更改为 [applyLabelAction](/graph/api/resources/applylabelaction?view=graph-rest-beta) 中的“label”****。 |
| 更改          | beta          | 已将“classificationIds”**** 属性更改为 [applyLabelAction](/graph/api/resources/applylabelaction?view=graph-rest-beta) 中的“responsibleSensitivityTypeIds”****。 |
| Addition        | beta          | 向 [applyLabelAction](/graph/api/resources/applylabelaction?view=graph-rest-beta) 添加了“actionSource”**** 属性。 |
| 更改          | beta          | 已将 [contentFormat](/graph/api/resources/enums?view=graph-rest-beta)) 枚举值“file”**** 更改为“default”****。 |
| 删除        | beta          | 已从 [actionSource](/graph/api/resources/enums?view=graph-rest-beta)) 枚举中删除“mandatory”**** 值。 |
| 更改          | beta          | 已将 [actionSource](/graph/api/resources/enums?view=graph-rest-beta)) 枚举值“policyDefault”**** 删除到“default”****。 |
| 删除        | beta          | 删除了“auditMetadataKey”****。 |
| 更改          | beta          | 已将“applyLabel”**** API 更改为 [evaluateApplication](/graph/api/informationprotectionlabel-evaluateapplication?view=graph-rest-beta)。 |
| 更改          | beta          | 已将“applyLabelFromClassification”**** API 更改为 [evaluateClassificationResults](/graph/api/informationprotectionlabel-evaluateclassificationresults?view=graph-rest-beta)。 |
| 更改          | beta          | 已将“removeLabel”**** API 更改为 [evaluateRemoval](/graph/api/informationprotectionlabel-evaluateremoval?view=graph-rest-beta). |
| 删除        | beta          | 已从 [extractLabel](/graph/api/informationprotectionlabel-extractlabel?view=graph-rest-beta) 删除“auditInfo”****。 |

### <a name="mail"></a>邮件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition        | Beta          | 向 [message](/graph/api/resources/message?view=graph-rest-beta) 实例[添加高达 150MB 的文件附件](outlook-large-attachments.md)。 |
| 添加        | Beta          | [attachmentItem](/graph/api/resources/attachmentitem?view=graph-rest-beta) 复杂类型、[attachment](/graph/api/resources/attachment?view=graph-rest-beta) 实体的 [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-beta) 操作和 **attachmentType** 枚举。 |
| 更改项         | Beta          | 扩展了 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 所使用的现有 [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta) 实体，以使其也适用于 **attachment**。 |

### <a name="notifications"></a>通知

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition        | Beta            |已添加[创建并发送通知](/graph/api/user-post-notifications?view=graph-rest-beta) API，以便无需管理代表令牌就可启用目标用户。 |
| 添加        | Beta          | 在 [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta) 资源上引入了“targetPolicy”**** 属性，以允许通过 webpush 定位 Web 终结点。 |
| 添加        | Beta            |  已在 [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta) 资源上添加了 **fallbackPolicy** 属性，以便为高优先级通知启用 iOS 上的保证传递。 |

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | Beta | 添加了[获取团队照片](/graph/api/team-get-photo?view=graph-rest-beta)和[更新团队照片](/graph/api/team-update-photo?view=graph-rest-beta)方法。 |
| 添加 | Beta | [读取邮件中的图像](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta)现在支持应用程序权限。 |

### <a name="users"></a>用户
| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition | v1.0 | 为 [user](/graph/api/resources/user?view=graph-rest-1.0) 资源添加了新的 **lastPasswordChangeDateTime** 属性。 |
| 添加项 | beta | 添加了 [user: reprocessLicenseAssignment API](/graph/api-reference/beta/api/user-reprocesslicense?view=graph-rest-beta)，它可用于重新处理[用户](/graph/api/resources/user?view=graph-rest-beta)的所有基于组的许可证分配。 |

### <a name="users--outlook-settings"></a>用户|Outlook 设置

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加项        | V1.0        | [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) 资源的 **dateFormat** 和 **timeFormat** 属性。 属性表示用户的首选日期和时间格式。|

## <a name="september-2019"></a>2019 年 9 月

### <a name="calendar-mail-groups"></a>日历, 邮件, 组

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition        | v1.0          | 向事件、消息或组帖子添加了[获取文件或项目附件的原始内容](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment)这一功能。 |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

|更改类型|版本|说明|
|:---|:---|:---|
|添加|beta|添加的新实体：<br/>[androidDeviceOwnerScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile)<br/>[androidManagedStoreWebApp](/graph/api/resources/intune-apps-androidmanagedstorewebapp)<br/>[appleEnrollmentProfileAssignment](/graph/api/resources/intune-enrollment-appleenrollmentprofileassignment)<br/>[appleUserInitiatedEnrollmentProfile](/graph/api/resources/intune-enrollment-appleuserinitiatedenrollmentprofile)<br/>[deviceCompliancePolicyPolicySetItem](/graph/api/resources/intune-policyset-devicecompliancepolicypolicysetitem)<br/>[deviceConfigurationPolicySetItem](/graph/api/resources/intune-policyset-deviceconfigurationpolicysetitem)<br/>[deviceManagementAutopilotEvent](/graph/api/resources/intune-troubleshooting-devicemanagementautopilotevent)<br/>[deviceManagementScriptPolicySetItem](/graph/api/resources/intune-policyset-devicemanagementscriptpolicysetitem)<br/>[enrollmentRestrictionsConfigurationPolicySetItem](/graph/api/resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem)<br/>[iosLobAppProvisioningConfigurationPolicySetItem](/graph/api/resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem)<br/>[macManagedAppProtection](/graph/api/resources/intune-policyset-macmanagedappprotection)<br/>[managedAppProtectionPolicySetItem](/graph/api/resources/intune-policyset-managedappprotectionpolicysetitem)<br/>[managedDeviceMobileAppConfigurationPolicySetItem](/graph/api/resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem)<br/>[mdmWindowsInformationProtectionPolicyPolicySetItem](/graph/api/resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem)<br/>[mobileAppPolicySetItem](/graph/api/resources/intune-policyset-mobileapppolicysetitem)<br/>[policySet](/graph/api/resources/intune-policyset-policyset)<br/>[policySetAssignment](/graph/api/resources/intune-policyset-policysetassignment)<br/>[policySetItem](/graph/api/resources/intune-policyset-policysetitem)<br/>[targetedManagedAppConfigurationPolicySetItem](/graph/api/resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem)<br/>[windows10EnrollmentCompletionPageConfigurationPolicySetItem](/graph/api/resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem)<br/>[windowsAutopilotDeploymentProfilePolicySetItem](/graph/api/resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem)<br/>[windowsFeatureUpdateProfile](/graph/api/resources/intune-softwareupdate-windowsfeatureupdateprofile)<br/>[windowsFeatureUpdateProfileAssignment](/graph/api/resources/intune-softwareupdate-windowsfeatureupdateprofileassignment)<br/>|
|添加项|beta|新增了复杂类型：<br/>[appleOwnerTypeEnrollmentType](/graph/api/resources/intune-enrollment-appleownertypeenrollmenttype)<br/>[configurationManagerAction](/graph/api/resources/intune-devices-configurationmanageraction)<br/>[credentialSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-credentialsinglesignonextension)<br/>[hasPayloadLinkResultItem](/graph/api/resources/intune-policyset-haspayloadlinkresultitem)<br/>[iosKerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-ioskerberossinglesignonextension)<br/>[kerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-kerberossinglesignonextension)<br/>[keyBooleanValuePair](/graph/api/resources/intune-deviceconfig-keybooleanvaluepair)<br/>[keyIntegerValuePair](/graph/api/resources/intune-deviceconfig-keyintegervaluepair)<br/>[keyRealValuePair](/graph/api/resources/intune-deviceconfig-keyrealvaluepair)<br/>[keyStringValuePair](/graph/api/resources/intune-deviceconfig-keystringvaluepair)<br/>[keyTypedValuePair](/graph/api/resources/intune-deviceconfig-keytypedvaluepair)<br/>[macOSKerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-macoskerberossinglesignonextension)<br/>[singleSignOnExtension](/graph/api/resources/intune-deviceconfig-singlesignonextension)<br/>|
|添加项|beta 版本|添加的新枚举类型：<br/>[appleUserInitiatedEnrollmentType](/graph/api/resources/intune-enrollment-appleuserinitiatedenrollmenttype)<br/>[bitLockerRecoveryPasswordRotationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype)<br/>[configurationManagerActionType](/graph/api/resources/intune-devices-configurationmanageractiontype)<br/>[deviceAndAppManagementAssignmentSource](/graph/api/resources/intune-shared-deviceandappmanagementassignmentsource)<br/>[errorCode](/graph/api/resources/intune-policyset-errorcode)<br/>[logLevel](/graph/api/resources/intune-troubleshooting-loglevel)<br/>[policySetStatus](/graph/api/resources/intune-policyset-policysetstatus)<br/>[userExperienceAnalyticsHealthState](/graph/api/resources/intune-devices-userexperienceanalyticshealthstate)<br/>[userExperienceAnalyticsInsightSeverity](/graph/api/resources/intune-devices-userexperienceanalyticsinsightseverity)<br/>[windowsAutopilotDeploymentState](/graph/api/resources/intune-troubleshooting-windowsautopilotdeploymentstate)<br/>[windowsAutopilotEnrollmentType](/graph/api/resources/intune-troubleshooting-windowsautopilotenrollmenttype)<br/>|
|添加项|beta|在 [policySet](/graph/api/resources/intune-policyset-policyset) 上添加了 [update](/graph/api/intune-policyset-policyset-update.md) 操作 |
|添加项|beta|在 [mobileApp](/graph/api/resources/intune-apps-mobileapp) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-mobileapp-haspayloadlinks.md) 操作 |
|添加项|beta|在 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md) 操作 |
|添加项|beta|在 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md) 操作 |
|添加项|beta|在 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-androidmanagedappprotection-haspayloadlinks.md) 操作 |
|Addition|beta|在 [macManagedAppProtection](/graph/api/resources/intune-policyset-macmanagedappprotection) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-macmanagedappprotection-haspayloadlinks.md) 操作 |
|添加项|beta|在 [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam-mdmwindowsinformationprotectionpolicy) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-mdmwindowsinformationprotectionpolicy-haspayloadlinks.md) 操作 |
|添加项|beta|在 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md) 操作 |
|添加项|beta|在 [policySet](/graph/api/resources/intune-policyset-policyset) 集合上添加了 [getPolicySets](/graph/api/intune-policyset-policyset-getpolicysets.md) 操作 |
|添加项|beta|在 [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-devicemanagementscript-haspayloadlinks.md) 操作 |
|添加项|beta|在 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-deviceconfiguration-haspayloadlinks.md) 操作 |
|添加项|beta|在 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-devicecompliancepolicy-haspayloadlinks.md) 操作 |
|添加项|beta|在 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md) 操作 |
|添加项|beta|在 [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration) 集合上添加了 [hasPayloadLinks](/graph/api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md) 操作 |
|添加项|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice) 上添加了 [triggerConfigurationManagerAction](/graph/api/intune-devices-manageddevice-triggerconfigurationmanageraction.md) 操作 |
|添加项|beta|在 [appleUserInitiatedEnrollmentProfile](/graph/api/resources/intune-enrollment-appleuserinitiatedenrollmentprofile) 上添加了 [setPriority](/graph/api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md) 操作 |
|添加项|beta|在 [windowsFeatureUpdateProfile](/graph/api/resources/intune-softwareupdate-windowsfeatureupdateprofile) 上添加了 [assign](/graph/api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md) 操作 |
|添加项|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting) 集合上添加了 [getExpiringVppTokenCount](o:getExpiringVppTokenCount:Collection(microsoft.graph.depOnboardingSetting)) 函数 |
|添加项|beta|向 [androidDeviceOwnerCompliancePolicy](/graph/api/resources/intune-deviceconfig-androiddeviceownercompliancepolicy) 实体添加了 **deviceThreatProtectionEnabled**、**deviceThreatProtectionRequiredSecurityLevel**、**securityRequireSafetyNetAttestationBasicIntegrity** 和 **securityRequireSafetyNetAttestationCertifiedDevice** 属性|
|添加项|beta|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration) 实体添加了 **workProfileAllowWidgets** 属性|
|添加项|beta|向 [androidManagedStoreApp](/graph/api/resources/intune-apps-androidmanagedstoreapp) 实体添加了 **isPrivate** 和 **isSystemApp** 属性|
|添加项|beta|向 [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration) 实体添加了 **workProfileAllowWidgets** 属性|
|添加项|beta|向 [depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile) 实体添加了 **screenTimeScreenDisabled** 属性|
|添加项|beta|向 [depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile) 实体添加了 **appearanceScreenDisabled**、**expressLanguageScreenDisabled**、**preferredLanguageScreenDisabled**、**deviceToDeviceMigrationDisabled** 和 **welcomeScreenDisabled** 属性|
|删除|beta|从 [depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile) 实体中删除了 **screenTimeScreenDisabled** 属性|
|添加项|beta|向 [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment) 实体添加了 **source** 和 **sourceId** 属性|
|删除|beta|从 [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript) 实体中删除了 **runRemediationScript** 属性|
|添加项|beta|向 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration) 实体添加了 **singleSignOnExtension** 属性|
|添加项|beta|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration) 实体添加了 **kioskModeEnableVoiceControl** 和 **kioskModeAllowVoiceControlModification** 属性|
|添加项|beta|向 [macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration) 实体添加了 **associatedDomains** 和 **singleSignOnExtension** 属性|
|添加项|beta|向 [targetedManagedAppPolicyAssignment](/graph/api/resources/intune-mam-targetedmanagedapppolicyassignment) 实体添加了 **source** 和 **sourceId** 属性|
|添加项|beta|向 [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [userExperienceAnalyticsBaseline](/graph/api/resources/intune-devices-userexperienceanalyticsbaseline) 实体添加了 **isBuiltIn** 和 **createdDateTime** 属性|
|删除|beta|从 [userExperienceAnalyticsBaseline](/graph/api/resources/intune-devices-userexperienceanalyticsbaseline) 实体中删除了 **overallScore** 和 **overallRegressionThreshold** 属性|
|删除|beta|从 [userExperienceAnalyticsCategory](/graph/api/resources/intune-devices-userexperienceanalyticscategory) 实体中删除了 **displayName** 和 **overallScore** 属性|
|删除|beta|从 [userExperienceAnalyticsMetric](/graph/api/resources/intune-devices-userexperienceanalyticsmetric) 实体中删除了 **displayName** 属性|
|删除|beta|从 [userExperienceAnalyticsOverview](/graph/api/resources/intune-devices-userexperienceanalyticsoverview) 实体中删除了 **overallScore**、**deviceBootPerformanceOverallScore** 和 **bestPracticesOverallScore** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration) 实体添加了 **attackSurfaceReductionRules** 和 **bitLockerRecoveryPasswordRotation** 属性|
|Addition|beta|向 [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration) 实体添加了 **trackInstallProgressForAutopilotOnly** 和 **disableUserStatusTrackingAfterFirstUser** 属性|
|添加项|beta|向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement) 实体添加了 **policySets** 导航属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement) 实体添加了 **appleUserInitiatedEnrollmentProfiles**、**autopilotEvents** 和 **windowsFeatureUpdateProfiles** 导航属性|
|添加项|beta|向 [insightValueDouble](/graph/api/resources/intune-devices-insightvaluedouble) 复杂类型添加了 **value** 属性|
|添加项|beta|向 [insightValueInt](/graph/api/resources/intune-devices-insightvalueint) 复杂类型添加了 **value** 属性|
|添加项|beta|向 [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem) 复杂类型添加了 **v13_0** 属性|
|添加项|beta|向 [macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem) 复杂类型添加了 **v10_14** 和 **v10_15** 属性|
|添加项|beta|向 [userExperienceAnalyticsInsight](/graph/api/resources/intune-devices-userexperienceanalyticsinsight) 复杂类型添加了 **values** 和 **severity** 属性|
|删除|beta|从 [userExperienceAnalyticsInsight](/graph/api/resources/intune-devices-userexperienceanalyticsinsight) 复杂类型中删除了 **value** 属性|
|添加项|beta 版本|向 [deviceEnrollmentType](/graph/api/resources/intune-shared-deviceenrollmenttype) 枚举类型添加了 **appleUserEnrollment**、**appleUserEnrollmentWithServiceAccount** 和 **appleUserEnrollmentWithAzureAD** 成员|
|添加项|beta 版本|向 [deviceManagementTemplateType](/graph/api/resources/intune-deviceintent-devicemanagementtemplatetype) 枚举类型添加了 **securityTemplate** 成员|
|添加项|beta 版本|向 [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction) 枚举类型添加了 **rebootNow** 成员|
|添加项|beta 版本|向 [remoteAction](/graph/api/resources/intune-devices-remoteaction) 枚举类型添加了 **rotateBitLockerKeys** 成员|
| 添加 | Beta | 添加了对写操作的应用程序权限支持：DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementRBAC.ReadWrite.All、DeviceManagementServiceConfig.ReadWrite.All |
| 添加项 | v1.0 | 向 [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem) 复杂类型添加了 **v13_0** 属性。 |

### <a name="education"></a>教育

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta | 向 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta) 添加了新属性 **closeDateTime**。|
| 更改 | beta | 在 [educationMakeCodeResource](/graph/api/resources/educationMakeCodeResource?view=graph-rest-beta) 资源中，已将属性名称 **mkcd** 更改为 **projectId** 并将 **url** 更改为 **hostWebUrl**。|

### <a name="cloud-communications--calls-and-online-meetings"></a>云通信 |呼叫和联机会议

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | Beta        | 为所有电话和网络会议添加了 /communications/* API。 路径 `/app` 已弃用。 今后，请使用路径 `/communications`。|
| 删除         | Beta        | 已弃用路径 `/app`。|
| 删除        | beta        | 已从资源 [commsOperation](/graph/.api/resource/commsOperation?view=graph-rest-beta) 中删除属性 **createdDateTime** 和 **lastActionDateTime**。|
| 删除        | beta        | 已从资源 [onlineMeeting](/graph/api/resources/onlineMeeting?view=graph-rest-beta) 中删除属性 **meetingType**。 |
| 添加        | Beta        | 将属性 **isBroadcast** 添加至资源 [onlineMeeting](/graph/api/resources/onlineMeeting?view=graph-rest-beta)。 |
| 更改        | Beta 版本        | 在资源 [commsNotification](/graph/api/resources/commsNotification?view=graph-rest-beta) 上将**资源**属性重命名为 **resourceUrl**。 |
| 更改          | Beta        | 在资源 [resultInfo](/graph/api/resources/resultInfo?view=graph-rest-beta) 上，将属性**code**和**subCode**的类型从字符串更改为 Int32。 |
| 更改        | Beta 版本        | 在资源 [resultInfo](/graph/api/resources/resultInfo?view=graph-rest-beta) 上将属性 **subcode** 重命名为 **subCode**。 |

### <a name="files"></a>文件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 添加了 [pendingOperations](/graph/api/resources/pendingOperations?view=graph-rest-beta) 和 [pendingContentUpdate](/graph/api/resources/pendingContentUpdate?view=graph-rest-beta) 资源。 **pendingOperations** 资源适用于 [driveItem](/graph/api/resources/driveItem?view=graph-rest-beta) 资源。 |
| 添加 | Beta | 向 [driveItem](/graph/api/resources/driveItem?view=graph-rest-beta) 资源添加了 [restore](/graph/api/driveitem-restore?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 向 [photo](/graph/api/resources/photo?view=graph-rest-beta) 资源添加了 **orientation** 属性。 |
| 添加 | Beta | 向 [hashes](/graph/api/resources/hashes?view=graph-rest-beta) 资源添加了 **sha256Hash** 属性。 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加 | Beta | 添加了 [objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-beta) 资源，它表示用于登录用户帐户的标识。 |
| 添加 | Beta | 向 [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta) 资源添加了 **synchronizationJobSettings** 属性。|
| 添加 | Beta | 为 [synchronizationQuarantine](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta) 资源中的 **reason** 属性添加了新的可能值。|
| Addition | Beta | 添加了在 [servicePrincipal 对象](/graph/api/resources/serviceprincipal?view=graph-rest-beta)上管理密码单一登录凭据的功能。 |

### <a name="mail"></a>邮件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项        | v1.0          | 添加了[获取消息的 MIME 内容](outlook-get-mime-message.md)的功能。 |

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 |beta| 向[团队](/graph/api/resources/team?view=graph-rest-beta)资源添加了 **primaryChannel** 属性。|
|Addition |beta| 向 [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta) 资源添加了 **allowCreatePrivateChannels** 属性。|

### <a name="users"></a>用户

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 资源添加了 **identities** 属性。 此属性表示此用户可用于登录的标识集。|
| 添加项        | v1.0          | 添加了 [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-1.0) 方法。|

### <a name="users--outlook-settings"></a>用户|Outlook 设置

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | Beta        | [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) 资源的 **dateFormat** 和 **timeFormat** 属性。 属性表示用户的首选日期和时间格式。|

## <a name="august-2019"></a>2019 年 8 月

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|添加的新实体：<br/>[androidDeviceOwnerCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androiddeviceownercertificateprofilebase?view=graph-rest-beta)<br/>[androidDeviceOwnerEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidDeviceOwnerTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate?view=graph-rest-beta)<br/>[androidDeviceOwnerVpnConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownervpnconfiguration?view=graph-rest-beta)<br/>[deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta)<br/>[userExperienceAnalyticsBaseline](/graph/api/resources/intune-devices-userexperienceanalyticsbaseline?view=graph-rest-beta)<br/>[userExperienceAnalyticsCategory](/graph/api/resources/intune-devices-userexperienceanalyticscategory?view=graph-rest-beta)<br/>[userExperienceAnalyticsMetric](/graph/api/resources/intune-devices-userexperienceanalyticsmetric?view=graph-rest-beta)<br/>[userExperienceAnalyticsOverview](/graph/api/resources/intune-devices-userexperienceanalyticsoverview?view=graph-rest-beta)<br/>[vpnConfiguration](/graph/api/resources/intune-deviceconfig-vpnconfiguration?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[configurationManagerClientInformation](/graph/api/resources/intune-devices-configurationmanagerclientinformation?view=graph-rest-beta)<br/>[deviceHealthScriptComplianceRule](/graph/api/resources/intune-devices-devicehealthscriptcompliancerule?view=graph-rest-beta)<br/>[insightValueDouble](/graph/api/resources/intune-devices-insightvaluedouble?view=graph-rest-beta)<br/>[insightValueInt](/graph/api/resources/intune-devices-insightvalueint?view=graph-rest-beta)<br/>[userExperienceAnalyticsInsight](/graph/api/resources/intune-devices-userexperienceanalyticsinsight?view=graph-rest-beta)<br/>[userExperienceAnalyticsInsightValue](/graph/api/resources/intune-devices-userexperienceanalyticsinsightvalue?view=graph-rest-beta)<br/>|
|添加项|beta 版本|添加的新枚举类型：<br/>[androidDeviceOwnerVirtualHomeButtonType](/graph/api/resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype?view=graph-rest-beta)<br/>[deviceHealthScriptComplianceRuleOperator](/graph/api/resources/intune-devices-devicehealthscriptcomplianceruleoperator?view=graph-rest-beta)<br/>[deviceHealthScriptDetectionType](/graph/api/resources/intune-devices-devicehealthscriptdetectiontype?view=graph-rest-beta)<br/>[powerActionType](/graph/api/resources/intune-deviceconfig-poweractiontype?view=graph-rest-beta)<br/>|
|添加项|beta|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 上添加了 [enableAndroidDeviceAdministratorEnrollment](/graph/api/intune-deviceconfig-devicemanagement-enableandroiddeviceadministratorenrollment?view=graph-rest-beta) 操作 |
|添加项|beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 集合新增了 executeAction 操作 |
|添加项|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [sendCustomNotificationToCompanyPortal](/graph/api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal?view=graph-rest-beta) 操作 |
|删除|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 集合上删除了 executeAction 操作 |
|添加项|beta|向 [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|删除|beta|从 [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) 实体中删除了 **scopeTags** 属性|
|添加项|beta|向 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **kioskModeScreenSaverConfigurationEnabled**、**kioskModeScreenSaverImageUrl**、**kioskModeScreenSaverDisplayTimeInSeconds**、**kioskModeScreenSaverStartDelayInSeconds**、**kioskModeScreenSaverDetectMediaDisabled**、**kioskModeVirtualHomeButtonType**、**kioskModeFlashlightConfigurationEnabled** 和 **kioskModeMediaVolumeConfigurationEnabled** 属性|
|添加项|beta|向 [deviceManagementScriptDeviceState](/graph/api/resources/intune-devices-devicemanagementscriptdevicestate?view=graph-rest-beta) 实体添加了 **lastSyncDateTime**、**preRemediationDetectionScriptOutput**、**remediationScriptError** 和 **postRemediationDetectionScriptOutput** 属性|
|添加项|beta|向 [deviceManagementScriptRunSummary](/graph/api/resources/intune-devices-devicemanagementscriptrunsummary?view=graph-rest-beta) 添加了 **compliantDeviceCount**、**notCompliantDeviceCount** 和 **pendingDeviceCount** 属性|
|添加项|beta|向 [intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta) 实体添加了 **isRemoveDeviceDisabled** 和 **isFactoryResetDisabled** 属性|
|添加项|beta|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **continuousPathKeyboardBlocked**、**findMyDeviceInFindMyAppBlocked**、**findMyFriendsInFindMyAppBlocked**、**wiFiBlockPowerModification** 和 **iTunesBlocked** 属性|
|添加项|beta|向 [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) 添加了 **iCloudBlockActivityContinuation** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **configurationManagerClientInformation** 属性|
|添加项|beta|向 [remoteActionAudit](/graph/api/resources/intune-devices-remoteactionaudit?view=graph-rest-beta) 实体添加了 **managedDeviceId** 属性|
|添加项|beta|向 [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) 实体添加了 **isBuiltIn** 属性|
|删除|beta|从 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体中删除了 **userRightsRegisterProcessAsService** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 添加了 **energySaverOnBatteryThresholdPercentage**、**energySaverPluggedInThresholdPercentage**、**powerLidCloseActionOnBattery**、**powerLidCloseActionPluggedIn**、**powerButtonActionOnBattery**、**powerButtonActionPluggedIn**、**powerSleepButtonActionOnBattery****powerSleepButtonActionPluggedIn**、**powerHybridSleepOnBattery** 和 **powerHybridSleepPluggedIn** 属性|
|添加项|beta|向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **deadlineForFeatureUpdatesInDays**、**deadlineForQualityUpdatesInDays**、**deadlineGracePeriodInDays** 和 **postponeRebootUntilAfterDeadline** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **userExperienceAnalyticsOverview**、**userExperienceAnalyticsBaselines** 和 **userExperienceAnalyticsCategories** 导航属性|
|删除|beta|从 [windowsManagementApp](/graph/api/resources/intune-devices-windowsmanagementapp?view=graph-rest-beta) 中删除了 **healthSummary** 导航属性||添加项|beta|向 [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta) 复杂类型添加了 **shareUserExperienceAnalyticsData** 属性|
|添加项|beta|向 [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta) 复杂类型添加了 **osBuildNumber** 属性|
|添加项|beta|向 [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) 复杂类型添加了 **isRemoveDeviceDisabled** 和 **isFactoryResetDisabled** 属性|
|添加项|beta|向 [iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta) 复杂类型添加了 **uninstallOnDeviceRemoval** 属性|
|添加项|beta|向 [iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta) 复杂类型添加了 **uninstallOnDeviceRemoval** 属性|
|添加项|beta|向 [iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta) 复杂类型添加了 **uninstallOnDeviceRemoval** 属性|
|添加项|beta|向 [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta) 枚举类型添加了 **customTextNotification** 成员|
|添加项|beta|向 [remoteAction](/graph/api/resources/intune-devices-remoteaction?view=graph-rest-beta) 枚举类型添加了 **setDeviceName** 成员|
|添加项|beta|向 [runState](/graph/api/resources/intune-shared-runstate?view=graph-rest-beta) 枚举类型添加了 **error** 和 **pending** 成员|
|添加项|beta|向 [weeklySchedule](/graph/api/resources/intune-deviceconfig-weeklyschedule?view=graph-rest-beta) 枚举类型添加了 **noScheduledScan** 成员|
|Addition|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement) 实体添加了 **derivedCredentials** 导航属性|

### <a name="education"></a>教育

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta | 向 [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta) 添加了新的属性 **grade**。|
| 添加项 | beta | 添加了新的 [educationRubric](/graph/api/resources/educationRubric?view=graph-rest-beta) 资源。|
| 添加项 | beta | 添加了用于管理 [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta) 和 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta) 上的 [educationRubric](/graph/api/resources/educationRubric?view=graph-rest-beta) 资源的 API。|
| 添加项 | beta | 添加了新的 [educationOutcome](/graph/api/resources/educationOutcome?view=graph-rest-beta) 资源。|
| 添加项 | beta | 添加了用于管理 [educationSubmission](/graph/api/resources/educationSubmission?view=graph-rest-beta) 上的 [educationOutcome](/graph/api/resources/educationOutcome?view=graph-rest-beta) 资源的 API。|
| 添加项 | beta | 添加了新的 [educationMakeCodeResource](/graph/api/resources/educationMakeCodeResource?view=graph-rest-beta) 资源。|
| 添加项    | beta    | 向 [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta) 添加了新的属性 **grade**。 |

### <a name="files"></a>文件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 上添加了 [unfollow](/graph/api/driveitem-unfollow?view=graph-rest-beta) 操作 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 更改 | Beta 版本 | 更改了[列出 provisioningObjectSummary](/graph/api/resources/provisioning-object-summary-list?view=graph-rest-beta) 命名空间。|
| 添加项 | Beta | 添加了 [roleManagement](/graph/api/resources/roleManagement?view=graph-rest-beta) 资源，可通过它访问 RBAC 提供商提供的角色定义和角色分配。 |
| 添加项 | Beta | 添加了 [unifiedRoleDefinition](/graph/api/resources/unifiedRoleDefinition?view=graph-rest-beta) 资源，它表示列出可执行的操作的权限列表。 |
| 添加 | Beta | 添加了 [unifiedRoleAssignment](/graph/api/resources/unifiedRoleAssignment?view=graph-rest-beta) 资源，它授予了访问资源的访问权限。 |
| 添加 | Beta | 添加了以下操作来支持 unifiedRoleDefinition 资源： <br><ul><li>[列出 unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta) - 获取面向提供商的 unifiedRoleDefinition 对象列表。</li><li>[创建 unifiedRoleDefinition](/graph/api/rbacapplication-post-roledefinitions?view=graph-rest-beta) - 创建新的 unifiedRoleDefinition 对象。</li><li>[获取 unifiedRoleDefinition](/graph/api/unifiedroledefinition-get?view=graph-rest-beta) - 检索统一角色定义对象的属性和关系。</li><li>[更新 unifiedRoleDefinition](/graph/api/unifiedroledefinition-update?view=graph-rest-beta) - 更新 unifiedRoleDefinition 对象的属性。</li><li>[删除 unifiedRoleDefinition](/graph/api/unifiedroledefinition-delete?view=graph-rest-beta) - 删除 unifiedRoleDefinition 对象。</li></ul> |
| 添加 | Beta | 添加了以下操作来支持 unifiedRoleAssignment 资源： <br><ul><li>[列出 unifiedRoleAssignments](/graph/api/rbacapplication-list-roleassignments?view=graph-rest-beta) - 获取面向提供商的 unifiedRoleAssignment 对象列表。</li><li>[创建 unifiedRoleAssignment]() -创建新的 unifiedRoleAssignment 对象。</li><li>[获取 unifiedRoleAssignment](/graph/api/unifiedroleassignment-get?view=graph-rest-beta) - 检索 unifiedRoleAssignment 对象的属性和关系。</li><li>[删除 unifiedRoleAssignment](/graph/api/unifiedroleassignment-delete?view=graph-rest-beta) -删除 unifiedRoleAssignment 对象。 |
| 添加 | Beta | 添加了[列出 accessReviews](/graph/api/accessreview-list?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 添加了[设备](/graph/api/resources/device?view=graph-rest-beta)资源的 [checkMemberObjects](/graph/api/device-checkmemberobjects?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 添加了 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) 资源的 [checkMemberObjects](/graph/api/directoryobject-checkmemberobjects?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 添加了 [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta) 资源的 [checkMemberObjects](/graph/api/directoryrole-checkmemberobjects?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 添加了[组](/graph/api/resources/group?view=graph-rest-beta)资源的 [checkMemberObjects](/graph/api/group-checkmemberobjects?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 添加了 [servicePrincipal](/graph/api/resources/serviceprinciple?view=graph-rest-beta) 资源的 [checkMemberObjects](/graph/api/serviceprincipal-checkmemberobjects?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 添加了[用户](/graph/api/resources/user?view=graph-rest-beta)资源的 [checkMemberObjects](/graph/api/user-checkmemberobjects?view=graph-rest-beta) 操作。 |
| 添加 | Beta | 添加了[用于读取组织联系人](permissions-reference.md#organizational-contact-permissions)的委派和应用程序权限：OrgContact.Read.All |
| 添加项 | beta | 添加了新实体 [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-beta)。 |
| 添加项 | beta | 添加了新的复杂类型 [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta)。 |
| Addition | beta | 在 [organization](/graph/api/resources/organization?view=graph-rest-beta) 资源上为 **certificateBasedAuthConfiguration** 添加了新的关系。 这将支持 [Azure Active Directory 中基于证书的身份验证](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)|

### <a name="reports"></a>报告

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加项        | v1.0  | 向 [mailboxUsageDetail](/graph/api/resources/mailboxUsageDetail?view=graph-rest-beta) 实体添加了 **deletedItemCount** 和 **deletedItemSizeInBytes** 属性。|
| 添加项        | v1.0  | 向 [office365GroupsActivityDetail](/graph/api/resources/office365GroupsActivityDetail?view=graph-rest-beta) 实体添加了 **groupId** 属性。|
| 添加项        | v1.0  | 向 [oneDriveUsageAccountDetail](/graph/api/resources/oneDriveUsageAccountDetail?view=graph-rest-beta) 实体添加了 **ownerPrincipalName** 属性。|
| 添加项        | v1.0  | 向 [sharePointSiteUsageDetail](/graph/api/resources/sharePointSiteUsageDetail?view=graph-rest-beta) 实体添加了 **ownerPrincipalName** 属性。|
| 添加项        | v1.0  | 已将 **office365Active** 和 **office365Inactive** 属性添加到 [office365ServicesUserCounts](/graph/api/resources/office365ServicesUserCounts?view=graph-rest-beta) 实体。|

### <a name="social-and-workplace-intelligence"></a>社交和工作场所智能

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | Beta | 引入了新的工作区智能[分析 API](/graph/api/resources/useranalytics?view=graph-rest-beta)，可便于分析用户如何在工作时间内和工作时间之外的各种活动上花费时间，包括电话、聊天（即时消息）、电子邮件、专注工作和会议。 |
| 添加 | Beta | 引入了新的工作区智能[设置 API](/graph/api/resources/settings?view=graph-rest-beta)，表示用户使用[分析 API](/graph/api/resources/useranalytics?view=graph-rest-beta) 所需的当前设置。 |
| 添加项 | Beta | 引入了新的 [activityStatistics](/graph/api/resources/activitystatistics?view=graph-rest-beta) 资源类型及其派生的以下新资源类型：[callActivityStatistics](/graph/api/resources/callactivitystatistics?view=graph-rest-beta)、[chatActivityStatistics](/graph/api/resources/chatactivitystatistics?view=graph-rest-beta)、[emailActivityStatistics](/graph/api/resources/emailactivitystatistics?view=graph-rest-beta)、[focusActivityStatistics](/graph/api/resources/focusactivitystatistics?view=graph-rest-beta) 和 [meetingActivityStatistics](/graph/api/resources/meetingactivitystatistics?view=graph-rest-beta)。 |

### <a name="tasks-and-plans"></a>任务和计划

|更改类型|版本|说明|
|:---|:---|:---|
|添加|Beta|向 [plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta) 实体添加了 **priority** 属性。|

### <a name="teamwork"></a>团队合作

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 添加了通过[频道消息 delta 查询 API](/graph/api/channel-messages-delta?view=graph-rest-beta) 从频道提取增量消息的功能。|
| 添加项 | Beta 版本 | 添加了[将成员添加到专用频道](/graph/api/conversationmember-add?view=graph-rest-beta)的功能。 |
| 添加项 | Beta 版本 | 添加了[从专用频道中删除成员](/graph/api/conversationmember-delete?view=graph-rest-beta)的功能。 |
| 添加项 | Beta 版本 | 添加了[更新专用频道中成员的角色](/graph/api/conversationmember-update?view=graph-rest-beta)这一功能。 |
| 新增 | Beta 版本 | 向[频道](/graph/api/resources/channel?view=graph-rest-beta)资源添加了 `membershipType` 属性来显示特定频道是专用频道还是标准频道。 |

## <a name="july-2019"></a>2019 年 7 月

### <a name="calendar--place"></a>日历 | 位置

首次推出位置 API，为应用中的位置提供丰富的细节。

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | Beta 版本  | 添加了[房间列表](/graph/api/resources/roomlist?view=graph-rest-beta)资源|
| 添加项        | Beta 版本  | 添加了[房间](/graph/api/resources/room?view=graph-rest-beta)资源|
| Addition        | Beta  | 添加了[位置](/graph/api/resources/place?view=graph-rest-beta)资源|
|添加项         | Beta  | [为位置 API 添加了委派和应用程序权限](permissions-reference.md#places-permissions)：Place.Read.All |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

|更改类型|版本|说明|
|:----------------|:------------|:-----------------------------------------|
|添加项|beta|添加的新实体：<br/>[managedAllDeviceCertificateState](/graph/api/resources/intune-deviceconfig-managedalldevicecertificatestate?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[windowsKioskForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windowskioskforceupdateschedule?view=graph-rest-beta)<br/>|
|添加项|beta 版本|添加的新枚举类型：<br/>[fileVaultState](/graph/api/resources/intune-deviceconfig-filevaultstate?view=graph-rest-beta)<br/>[windowsDefenderTamperProtectionOptions](/graph/api/resources/intune-deviceconfig-windowsdefendertamperprotectionoptions?view=graph-rest-beta)<br/>|
|添加项|beta|在 [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) 集合上添加了 getRoleScopeTagsById 操作 |
|添加项|beta|在 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 上添加了 [createInstance](/graph/api/intune-deviceintent-devicemanagementtemplate-createinstance?view=graph-rest-beta) 操作 |
|添加项|beta|在 [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) 集合上添加了 hasCustomRoleScopeTag 函数 |
|删除|beta|已删除 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 上的 [createInstance](/graph/api/intune-deviceintent-devicemanagementtemplate-createinstance?view=graph-rest-beta) 操作 |
|删除|beta|已删除 [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) 上的 [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) 函数 |
|添加项|beta|向 [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) 实体添加了 **scopeTags** 属性|
|添加项|beta|向 [androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta) 实体添加了 **nestedSchemaItems** 属性|
|添加项|beta|向 [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **groupTag** 属性|
|添加项|beta|向 [managedDeviceEncryptionState](/graph/api/resources/intune-deviceconfig-manageddeviceencryptionstate?view=graph-rest-beta) 实体添加了 **fileVaultStates** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **userRightsDenyLocalLogOn** 和 **windowsDefenderTamperProtection** 属性|
|添加项|beta|向 [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) 实体添加了 **localGuestAccountName** 和 **assessmentAppUserModelId** 属性|
|添加项|beta|向 [windowsDeliveryOptimizationConfiguration](/graph/api/resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration?view=graph-rest-beta) 实体添加了 **cacheServerHostNames**、**cacheServerForegroundDownloadFallbackToHttpDelayInSeconds** 和 **cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds** 属性|
|添加项|beta|向 [windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta) 实体添加了 **windowsKioskForceUpdateSchedule** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceConfigurationsAllManagedDeviceCertificateStates** 导航属性|
|删除|beta|从 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体中删除了 **importedWindowsAutopilotDeviceIdentityUploads** 导航属性|
|添加项|beta|向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **deviceUpdateStates** 属性|
|添加项|beta|向 [androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta) 复杂类型添加了 **index** 和 **parentIndex** 属性|
|添加项|beta|向 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型添加了 **androidDeviceAdministratorEnrollmentEnabled** 属性|
|添加项|beta|向 [windowsFirewallRule](/graph/api/resources/intune-deviceconfig-windowsfirewallrule?view=graph-rest-beta) 复杂类型添加了 **edgeTraversal** 属性|
|添加项|beta|向 [secureAssessmentAccountType](/graph/api/resources/intune-deviceconfig-secureassessmentaccounttype?view=graph-rest-beta) 枚举类型添加了 **localGuestAccount** 成员|
|添加项|beta|向 [vpnLocalIdentifier](/graph/api/resources/intune-deviceconfig-vpnlocalidentifier?view=graph-rest-beta) 枚举类型添加了 **empty** 和 **clientCertificateSubjectName** 成员|
|添加项|beta|将 **revision** 属性添加到了 [groupPolicyDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicydefinitionfile?view=graph-rest-beta) 实体|
|添加项|beta|将 **valuePrefix** 属性添加到了 [groupPolicyPresentationListBox](/graph/api/resources/intune-grouppolicy-grouppolicypresentationlistbox?view=graph-rest-beta) 实体|

### <a name="files-onedrive-for-business"></a>文件 (OneDrive for Business)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|向 [createLink](/graph/api/driveitem-createlink?view=graph-rest-beta) 操作添加了 **expirationDatetime** 和 **password** 属性。 |

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加项 | v1.0 | 添加了[新的委派和应用程序权限](/graph/permissions-reference?#organization-permissions) _Organization.Read.All_ 和 _Organization.ReadWrite.All_，以获取并更新[组织 API](/graph/api/resources/organization?view=graph-rest-1.0) 资源以及获取 [subcribedSku](/graph/api/resources/subscribedSku?view=graph-rest-1.0) 资源。 |
| 添加 | Beta | 添加了[新的委派和应用程序权限](/graph/permissions-reference?#organization-permissions) _Organization.Read.All_ 和 _Organization.ReadWrite.All_，以获取并更新[组织 API](/graph/api/resources/organization?view=graph-rest-beta) 资源以及获取 [subcribedSku](/graph/api/resources/subscribedSku?view=graph-rest-beta) 资源。 |
| 添加项 | v1.0 | 在[组](/graph/api/group-delta?view=graph-rest-1.0)中添加了 [group:validateProperties 函数](/graph/api/group-validateproperties?view=graph-rest-1.0)和 [directoryobject:validateProperties 函数](/graph/api/group-validateproperties?view=graph-rest-1.0)，用于验证 Office 365 组的显示名称或邮件别名是否符合命名策略。 |
| 添加 | Beta |向资源类型 [directoryDefinition](/graph/api/resources/synchronization-directorydefinition?view=graph-rest-beta) 添加了“version”、“discoveryDateTime”和“discoverabilities”属性。|
| 添加 | Beta |添加了 [directoryDefinition: discover](/graph/api/resources/directorydefinition-discover?view=graph-rest-beta) 方法。|
| 添加 | Beta | 添加了[新的委派和应用程序权限](/graph/permissions-reference?#organization-permissions) _AdministrativeUnit.Read.All_ 和 _AdministrativeUnit.ReadWrite.All_，以获取和更新[管理单元 API](/graph/api/resources/administrativeunit?view=graph-rest-beta) 资源。 |
| 添加项 | v1.0 | 添加了[新的委派和应用程序权限](/graph/permissions-reference?#organization-permissions) _RoleManagement.Read.Directory_ 和 _RoleManagement.ReadWrite.Directory_以获取和更新[目录角色 API](/graph/api/resources/directoryRole?view=graph-rest-1.0) 资源并获取[目录角色模板 API](/graph/api/resources/directoryRoleTemplate?view=graph-rest-1.0) 资源。 |
| 添加 | Beta | 添加了[新的应用程序权限](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_，以在[访问评审 API](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 中执行获取、创建、更新和删除操作。 |
| 添加 | Beta | 向[目录](/graph/api/resources/directory?view=graph-rest-beta)资源添加了新的资源类型 [**featureRolloutPolicy**](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta)。 功能推出策略可帮助租户管理员在为整个组织启用一些功能之前，针对特定组试用这些功能。|


### <a name="mail-outlook"></a>邮件 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 增加了对 mailFolder API 中 Mail.ReadBasic.All 权限的支持：[list mailfolders](/graph/api/user-list-mailfolders?view=graph-rest-beta)、[get a mailfolder](/graph/api/mailfolder-get?view=graph-rest-beta)、[list child folders](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta) 和 [list messages in a mail folder](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta)。 还在 [delta query for message](/graph/api/message-delta?view=graph-rest-beta) 和 [delta query for mailFolder](/graph/api/mailfolder-delta?view=graph-rest-beta) 中添加了 Mail.ReadBasic.All 支持。|

### <a name="sites-sharepoint"></a>网站 (SharePoint)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | beta        | 向 [list](/graph/api/resources/list?view=graph-rest-beta) 实体添加了 **subscriptions** 导航属性。 |

### <a name="reports"></a>报告

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| Addition        | Beta  | 向 [mailboxUsageDetail](/graph/api/resources/mailboxUsageDetail?view=graph-rest-beta) 实体添加了 **deletedItemCount** 属性。|
| 添加        | Beta  | 向 [mailboxUsageDetail](/graph/api/resources/mailboxUsageDetail?view=graph-rest-beta) 实体添加了 **deletedItemSizeInBytes** 属性。|
| 添加        | Beta  | 向 [office365GroupsActivityDetail](/graph/api/resources/office365GroupsActivityDetail?view=graph-rest-beta) 实体添加了 **groupId** 属性。|

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 添加了对[列出频道消息](/graph/api/channel-list-messages?view=graph-rest-beta)，[获取频道消息](/graph/api/channel-get-message?view=graph-rest-beta)，[列出消息回复](/graph/api/channel-list-messagereplies?view=graph-rest-beta)，以及[获取消息回复](/graph/api/channel-get-messagereply?view=graph-rest-beta)的应用程序权限的支持。 |
| 添加项 | beta | 添加了对[在聊天中列出消息](/graph/api/chatmessage-list?view=graph-rest-beta)和[在聊天中获取消息](/graph/api/chatmessage-get?view=graph-rest-beta)的应用程序权限的支持。 |
| 添加项 | beta | 已将**installedApps**属性添加到[聊天](/graph/api/resources/chat?view=graph-rest-beta)资源。|
| 添加项 | beta | 已添加**用户** 资源的"[聊天](/graph/api/resources/user?view=graph-rest-beta)"属性的导航绑定。|
| 添加项 | beta | 添加了[团队合作](/graph/api/resources/teamwork?view=graph-rest-beta)的资源。 |
| 添加项 | beta | 添加了[userTeamwork](/graph/api/resources/userteamwork?view=graph-rest-beta)的资源。 |
| 添加项 | beta | 向[用户](/graph/api/resources/user?view=graph-rest-beta)资源添加了新方法，为用户个人应用启用以下方法： <br>[列出为用户安装的应用](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) <br>[为用户安装应用](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta) <br>[为用户卸载应用](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta) <br>[升级为用户安装的应用](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta)|

### <a name="calls-and-online-meetings"></a>呼叫和联机会议

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | Beta        | 向[呼叫](/api-reference/beta/resources/call.md)资源添加了 **mediaState** 属性|
| 更改          | Beta 版本        | 已将 [recordOperation](/api-reference/beta/resources/recordOperation.md) 资源中的 **recordResourceLocation** 属性重命名为 **recordingLocation**|
| 更改          | Beta 版本        | 已将 [recordOperation](/api-reference/beta/resources/recordOperation.md) 资源中的 **recordResourceAccessToken** 属性重命名为 **recordingAccessToken**|
| 添加项        | Beta        | 向 [onlineMeeting](/api-reference/beta/resources/onlinemeeting.md) 资源添加了 **capabilities** 属性 |
| 添加项        | Beta        | 向 [onlineMeeting](/api-reference/beta/resources/onlinemeeting.md) 资源添加了 **videoTeleconferenceId** 属性 |
| 添加项        | Beta        | 向 [meetingParticipants](/api-reference/beta/resources/meetingparticipants.md) 资源添加了 **producers** 属性 |
| 添加项        | Beta        | 向 [meetingParticipants](/api-reference/beta/resources/meetingparticipants.md) 资源添加了 **contributors** 属性 |

## <a name="june-2019"></a>2019 年 6 月

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|添加的新实体：<br/>[appVulnerabilityManagedDevice](/graph/api/resources/intune-partnerintegration-appvulnerabilitymanageddevice?view=graph-rest-beta)<br/>[appVulnerabilityMobileApp](/graph/api/resources/intune-partnerintegration-appvulnerabilitymobileapp?view=graph-rest-beta)<br/>[appVulnerabilityTask](/graph/api/resources/intune-partnerintegration-appvulnerabilitytask?view=graph-rest-beta)<br/>[deviceAppManagementTask](/graph/api/resources/intune-partnerintegration-deviceappmanagementtask?view=graph-rest-beta)<br/>[deviceManagementDomainJoinConnector](/graph/api/resources/intune-odj-devicemanagementdomainjoinconnector?view=graph-rest-beta)<br/>[iosikEv2VpnConfiguration](/graph/api/resources/intune-deviceconfig-iosikev2vpnconfiguration?view=graph-rest-beta)<br/>[roleScopeTagAutoAssignment](/graph/api/resources/intune-rbac-rolescopetagautoassignment?view=graph-rest-beta)<br/>[windows10DeviceFirmwareConfigurationInterface](/graph/api/resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[deviceManagementApplicabilityRuleDeviceMode](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode?view=graph-rest-beta)<br/>[deviceManagementApplicabilityRuleOsEdition](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition?view=graph-rest-beta)<br/>[deviceManagementApplicabilityRuleOsVersion](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion?view=graph-rest-beta)<br/>[deviceManagementSettingComparison](/graph/api/resources/intune-deviceintent-devicemanagementsettingcomparison?view=graph-rest-beta)<br/>[iosVpnSecurityAssociationParameters](/graph/api/resources/intune-deviceconfig-iosvpnsecurityassociationparameters?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新枚举类型：<br/>[appInstallControlType](/graph/api/resources/intune-deviceconfig-appinstallcontroltype?view=graph-rest-beta)<br/>[appVulnerabilityTaskMitigationType](/graph/api/resources/intune-partnerintegration-appvulnerabilitytaskmitigationtype?view=graph-rest-beta)<br/>[changeUefiSettingsPermission](/graph/api/resources/intune-deviceconfig-changeuefisettingspermission?view=graph-rest-beta)<br/>[deviceAppManagementTaskCategory](/graph/api/resources/intune-partnerintegration-deviceappmanagementtaskcategory?view=graph-rest-beta)<br/>[deviceAppManagementTaskPriority](/graph/api/resources/intune-partnerintegration-deviceappmanagementtaskpriority?view=graph-rest-beta)<br/>[deviceAppManagementTaskStatus](/graph/api/resources/intune-partnerintegration-deviceappmanagementtaskstatus?view=graph-rest-beta)<br/>[deviceManagementApplicabilityRuleType](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruletype?view=graph-rest-beta)<br/>[deviceManagementComparisonResult](/graph/api/resources/intune-deviceintent-devicemanagementcomparisonresult?view=graph-rest-beta)<br/>[deviceManagementDomainJoinConnectorState](/graph/api/resources/intune-odj-devicemanagementdomainjoinconnectorstate?view=graph-rest-beta)<br/>[deviceManagementTemplateType](/graph/api/resources/intune-deviceintent-devicemanagementtemplatetype?view=graph-rest-beta)<br/>[macOSFileVaultRecoveryKeyTypes](/graph/api/resources/intune-deviceconfig-macosfilevaultrecoverykeytypes?view=graph-rest-beta)<br/>[managedAppNotificationRestriction](/graph/api/resources/intune-mam-managedappnotificationrestriction?view=graph-rest-beta)<br/>[mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>[secureBootWithDMAType](/graph/api/resources/intune-deviceconfig-securebootwithdmatype?view=graph-rest-beta)<br/>[vpnClientAuthenticationType](/graph/api/resources/intune-deviceconfig-vpnclientauthenticationtype?view=graph-rest-beta)<br/>[vpnDeadPeerDetectionRate](/graph/api/resources/intune-deviceconfig-vpndeadpeerdetectionrate?view=graph-rest-beta)<br/>[vpnEncryptionAlgorithmType](/graph/api/resources/intune-deviceconfig-vpnencryptionalgorithmtype?view=graph-rest-beta)<br/>[vpnIntegrityAlgorithmType](/graph/api/resources/intune-deviceconfig-vpnintegrityalgorithmtype?view=graph-rest-beta)<br/>[vpnLocalIdentifier](/graph/api/resources/intune-deviceconfig-vpnlocalidentifier?view=graph-rest-beta)<br/>[vpnServerCertificateType](/graph/api/resources/intune-deviceconfig-vpnservercertificatetype?view=graph-rest-beta)<br/>[windows10DeviceModeType](/graph/api/resources/intune-deviceconfig-windows10devicemodetype?view=graph-rest-beta)<br/>|
|Addition|beta|在 [deviceAppManagementTask](/graph/api/resources/intune-partnerintegration-deviceappmanagementtask?view=graph-rest-beta) 上添加了 [updateStatus](/graph/api/intune-partnerintegration-deviceappmanagementtask-updatestatus?view=graph-rest-beta) 操作 |
|添加项|beta|在 [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-rbac-rolescopetag-assign?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 上添加了 [compare](/graph/api/intune-deviceintent-devicemanagementtemplate-compare?view=graph-rest-beta) 函数 |
|添加项|beta|在 [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) 上添加了 [compare](/graph/api/intune-deviceintent-devicemanagementintent-compare?view=graph-rest-beta) 函数 |
|删除|beta|删除了以下枚举类型：<br/>**mobileAppDependecyType**<br/>|
|添加项|beta|向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 实体添加了 **deviceManagementApplicabilityRuleOsEdition**、**deviceManagementApplicabilityRuleOsVersion** 和 **deviceManagementApplicabilityRuleDeviceMode** 属性|
|添加项|beta|向 [deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **securityKeyForSignIn** 属性|
|添加项|beta|向 [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 实体添加了 **templateType** 和 **publishedDateTime** 属性|
|添加项|beta|向 [intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta) 实体添加了 **customPrivacyMessage** 属性|
|添加项|beta|向 [macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **fileVaultEnabled**、**fileVaultSelectedRecoveryKeyTypes**、**fileVaultInstitutionalRecoveryKeyCertificate**、**fileVaultInstitutionalRecoveryKeyCertificateFileName**、**fileVaultPersonalRecoveryKeyHelpMessage**、**fileVaultAllowDeferralUntilSignOut**、**fileVaultNumberOfTimesUserCanIgnore**、**fileVaultDisablePromptAtSignOut** 和 **fileVaultPersonalRecoveryKeyRotationInMonths** 属性|
|添加项|beta|向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体添加了 **notificationRestriction** 属性|
|更改|beta|更改了 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **dependencyType** 从 [mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta) 更改成了 [mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **deviceGuardSecureBootWithDMA** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **smartScreenAppInstallControl** 和 **lockScreenActivateAppsWithVoice** 属性|
|添加项|beta|向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **deviceAppManagementTasks** 导航属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **domainJoinConnectors** 导航属性|
|添加项|beta|向 [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) 实体添加了 **assignments** 导航属性|
|添加项|beta|向 [omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-beta) 复杂类型添加了 **isReadOnly** 属性|
|添加项|beta|向 [windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta) 复杂类型添加了 **v10_1809** 和 **v10_1903** 属性|
|添加项|beta|向 [androidWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androidwifisecuritytype?view=graph-rest-beta) 枚举类型添加了 **wpa2Enterprise** 成员|
|添加项|beta|向 [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **ikEv2** 成员|
|添加项|beta|向 [remoteAction](/graph/api/resources/intune-devices-remoteaction?view=graph-rest-beta) 枚举类型添加了 **rotateFileVaultKey** 和 **getFileVaultKey** 成员|
|添加项|beta|向 [vpnAuthenticationMethod](/graph/api/resources/intune-deviceconfig-vpnauthenticationmethod?view=graph-rest-beta) 枚举类型添加了 **sharedSecret** 成员|
|添加项|beta|向 [windows10EditionType](/graph/api/resources/intune-deviceconfig-windows10editiontype?view=graph-rest-beta) 枚举类型添加了 **windows10Home**、**windows10HomeChina**、**windows10HomeN**、**windows10HomeSingleLanguage**、**windows10Mobile**、**windows10IoTCore** 和 **windows10IoTCoreCommercial** 成员|

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加项 | beta | 添加了 [riskDetection API](/graph/api/resources/riskdetection?view=graph-rest-beta)，它表示 Azure AD Identity Protection 中的风险检测。 |
| 添加        | Beta  | 引入了新资源类型 [applicationTemplate](/graph/api/resources/applicationtemplate.md)。 此资源类型支持从 Azure AD 应用程序库[实例化](/graph/api/applicationtemplate-instantiate.md)、[列出](/graph/api/applicationtemplate-instantiate.md)和[获取](/graph/api/applicationtemplate-get.md)应用程序。|
| 添加项 | beta|添加了新资源： </br> [detailsInfo](/graph/api/resources/detailsInfo?view=graph-rest-beta)</br> [initiator](/graph/api/resources/initiator?view=graph-rest-beta)</br> [modifiedProperty](/graph/api/resources/modifiedProperty?view=graph-rest-beta)</br> [provisionedIdentity](/graph/api/resources/provisionedIdentity?view=graph-rest-beta)</br> [provisioningObjectsummary](/graph/api/resources/provisioningObjectsummary?view=graph-rest-beta)</br> [provisioningStep](/graph/api/resources/provisioningStep?view=graph-rest-beta)</br> [provisioningsystemDetails](/graph/api/resources/provisioningsystemDetails?view=graph-rest-beta)</br> [statusBase](/graph/api/resources/statusBase?view=graph-rest-beta)|
| 添加项 |beta |添加了 [List provisioningObjectSummary](/graph/api/resources/provisioning-object-summary-list?view=graph-rest-beta) 操作</br>|                     |
| 添加项 | v1.0 | 在[用户](/graph/api/resources/user?view=graph-rest-1.0)资源上添加了 **signInSessionsValidFromDateTime** 属性。 |
| 添加项 | v1.0 | 在[用户](/graph/api/resources/user?view=graph-rest-1.0)资源上添加了 [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) 操作。 |

### <a name="mail-outlook"></a>邮件 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta | 增加了对 mailFolder API 中 Mail.ReadBasic 权限的支持：[list mailfolders](/graph/api/user-list-mailfolders?view=graph-rest-beta)、[get a mailfolder](/graph/api/mailfolder-get?view=graph-rest-beta)、[list child folders](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta) 和 [list messages in a mail folder](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta)。 还在 [delta query for message](/graph/api/message-delta?view=graph-rest-beta) 和 [delta query for mailFolder](/graph/api/mailfolder-delta?view=graph-rest-beta) 中添加了 Mail.ReadBasic 支持。|

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|添加|beta| 添加了用于检索用户注册和使用情况信息的新报表：<br/><ul><li>[reportroot-getcredentialusagesummary](/graph/api/reportroot-getcredentialusagesummary?view=graph-rest-beta) - 报告自助服务密码重置的使用情况。</li><li>[reportroot-getcredentialuserregistrationcount](/graph/api/reportroot-getcredentialuserregistrationcount?view=graph-rest-beta) - 报告自助服务密码重置和多重身份验证的注册数量。</li><li>[reportroot-list-credentialuserregistrationdetails](/graph/api/reportroot-list-credentialuserregistrationdetails?view=graph-rest-beta) - 报告自助服务密码重置和多重身份验证的使用情况。</li><li>[reportroot-list-usercredentialusagedetails](/graph/api/resources/reportroot-list-usercredentialusagedetails?view=graph-rest-beta) - 报告某个用户的自助式密码重置的使用情况。</li></ul> |

### <a name="sites-and-lists-sharepoint"></a>网站和列表 (SharePoint)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 实体集添加了 [followSite](/graph/api/follow-site?view=graph-rest-beta) 导航属性 |
| 添加项        | Beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 实体集添加了 [unfollowSite](/graph/api/unfollow-site?view=graph-rest-beta) 导航属性 |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | beta | 添加了 [teamDiscoverySettings](/api-reference/beta/resources/teamdiscoverysettings.md) 资源和相关方法。 |

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 为 [user](/graph/api/resources/user?view=graph-rest-beta) 实体添加了 **lastPasswordChangeDateTime** 属性。 |

## <a name="may-2019"></a>2019 年 5 月

### <a name="calendar-mail-personal-contacts-outlook"></a>日历、邮件和个人联系人 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | v1.0 和 beta | 添加了管理员限制应用程序仅访问特定邮箱的功能，即使应用程序已被授予邮件、邮箱设置、日历或联系人的应用程序权限。 有关更多详细信息，请参阅[将应用程序权限界定为特定 Exchange Online 邮箱](auth-limit-mailbox-access.md)。 |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|加|beta|添加的新实体：<br/>[deviceManagementDerivedCredentialSettings](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialsettings?view=graph-rest-beta)<br/>[iosDerivedCredentialAuthenticationConfiguration](/graph/api/resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration?view=graph-rest-beta)<br/>[securityBaselineCategoryStateSummary](/graph/api/resources/intune-deviceintent-securitybaselinecategorystatesummary?view=graph-rest-beta)<br/>|
|加|beta|添加的新枚举类型：<br/>[deviceManagementDerivedCredentialIssuer](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialissuer?view=graph-rest-beta)<br/>[deviceManagementDerivedCredentialNotificationType](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype?view=graph-rest-beta)<br/>[emailCertificateType](/graph/api/resources/intune-deviceconfig-emailcertificatetype?view=graph-rest-beta)<br/>[mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>|
|加|beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 集合新增了 executeAction 操作 |
|加|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [rotateFileVaultKey](/graph/api/intune-devices-manageddevice-rotatefilevaultkey?view=graph-rest-beta) 操作 |
|加|beta|在 [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) 上添加了 [migrateToTemplate](/graph/api/intune-deviceintent-devicemanagementintent-migratetotemplate?view=graph-rest-beta) 操作 |
|加|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [getFileVaultKey](/graph/api/intune-devices-manageddevice-getfilevaultkey?view=graph-rest-beta) 函数 |
|删除|beta|删除了以下枚举类型：<br/>**mobileAppDependecyType**<br/>|
|删除|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 集合上删除了 executeAction 操作 |
|加|beta|向 [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **usernameFormatString**、**passwordFormatString** 和 **preSharedKey** 属性|
|加|beta|向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **customBrowserPackageId** 和 **customBrowserDisplayName** 属性|
|加|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **customBrowserProtocol**、**customBrowserPackageId** 和 **customBrowserDisplayName** 属性|
|删除|beta|从 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体中删除了 **thirdPartyKeyboardsBlocked** 属性|
|更改|beta|在 [deviceManagementAbstractComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance?view=graph-rest-beta) 实体上更改了以下属性：<br/>将 **implementationId** 从必需更改为可选<br/>|
|添加项|beta|向 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 实体添加了 **versionInfo**、**isDeprecated** 和 **intentCount** 属性|
|加|beta|向 [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **assignedUserPrincipalName** 属性|
|添加项|beta|向 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体添加了 **signingCertificateType** 和 **encryptionCertificateType** 属性|
|添加项|beta|向 [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **usernameFormatString** 和 **passwordFormatString** 属性|
|添加项|beta|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **kioskModeBlockAutoLock**、**kioskModeBlockRingerSwitch**、**kioskModeBlockScreenRotation**、**kioskModeBlockSleepButton**、**kioskModeBlockTouchscreen**、**cellularBlockPersonalHotspotModification** 和 **siriDisableServerLogging** 属性|
|添加项|beta|向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **customBrowserProtocol** 属性|
|删除|beta|从 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体中删除了 **thirdPartyKeyboardsBlocked** 属性|
|添加项|beta|向 [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **iCloudBlockPhotoLibrary**、**screenCaptureBlocked**、**classroomAppBlockRemoteScreenObservation**、**classroomAppForceUnpromptedScreenObservation**、**classroomForceAutomaticallyJoinClasses**、**classroomForceRequestPermissionToLeaveClasses** 和 **classroomForceUnpromptedAppAndDeviceLock** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **retireAfterDateTime** 属性|
|更改|beta|更改了 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **dependencyType** 从 [mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta) 更改成了 [mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>|
|添加项|beta|向 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 属性添加了 **tpmRequired** 属性|
|添加项|beta|向 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [windowsHealthMonitoringConfiguration](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringconfiguration?view=graph-rest-beta) 实体添加了 **configDeviceHealthMonitoringCustomScope** 属性|
|添加项|beta|向 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 实体添加了 **migratableTo** 导航属性|
|添加项|beta|向 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体添加了 **derivedCredentialSettings** 导航属性|
|添加项|beta|向 [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **derivedCredentialSettings** 导航属性|
|添加项|beta|向 [iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta) 实体添加了 **derivedCredentialSettings** 导航属性|
|添加项|beta|向 [securityBaselineTemplate](/graph/api/resources/intune-deviceintent-securitybaselinetemplate?view=graph-rest-beta) 实体添加了 **categoryDeviceStateSummaries** 导航属性|
|添加项|beta|向 [androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta) 枚举类型添加了 **wpaEnterprise** 成员|
|添加项|beta|向 [devicePlatformType](/graph/api/resources/intune-shared-deviceplatformtype?view=graph-rest-beta) 枚举类型添加了 **unknown** 成员|
|添加项|beta|向 [easAuthenticationMethod](/graph/api/resources/intune-deviceconfig-easauthenticationmethod?view=graph-rest-beta) 枚举类型添加了 **derivedCredential** 成员|
|添加项|beta|向 [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta) 枚举类型添加了 **wipe** 成员|
|更改|beta|更改了 [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta) 枚举类型上以下属性的类型：<br/>将 **fullScan** 从 2 更改成了 3<br/>将 **quickScan** 从 3 更改成了 4<br/>将 **signatureUpdate** 从 4 更改成了 5<br/>|
|添加项|beta|向 [vpnAuthenticationMethod](/graph/api/resources/intune-deviceconfig-vpnauthenticationmethod?view=graph-rest-beta) 枚举类型添加了 **derivedCredential** 成员|
|添加项|beta|向 [wiFiAuthenticationMethod](/graph/api/resources/intune-deviceconfig-wifiauthenticationmethod?view=graph-rest-beta) 枚举类型添加了 **derivedCredential** 成员|

### <a name="files-onedrive"></a>文件 (OneDrive)
| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 已添加[捆绑](/graph/api/resources/bundle?view=graph-rest-beta)复杂类型 |
| 添加项 | Beta | 已添加[相册](/graph/api/resources/album?view=graph-rest-beta)复杂类型 |
| 添加项 | Beta | 向[drive](/graph/api/resources/drive?view=graph-rest-beta) 实体添加了**捆绑** 导航属性 |
| 添加项 | Beta | 向 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 实体添加了 **捆绑** 属性 |
| 添加项 | Beta | 已向[权限](/graph/api/resources/permission?view=graph-rest-beta)实体添加**授予**操作 |

### <a name="education"></a>教育
| 更改类型 | 版本 | 说明                                                                                                                                                      |
| :---------- | :------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 添加项    | beta    | 已将 taughtClasses 添加到 [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta)。                                                                  |
| 添加项    | beta    | 已[将](/graph/api/resources/educationCourse?view=graph-rest-beta) educationCourse [添加到 educationClass](/graph/api/resources/educationClass?view=graph-rest-beta)。 |
| 添加项    | beta    | 向 [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta)添加了[delta](/graph/delta-query-overview)支持。                                   |
| 添加项    | beta    | 已向 [educationSchool](/graph/api/resources/educationSchool?view=graph-rest-beta) 添加 [delta](/graph/delta-query-overview)。                                       |
| 添加项    | beta    | 已向 [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta) 添加 [delta](/graph/delta-query-overview)。                                         |
| 添加项    | beta    | 已向 [educationUserRole](/graph/api/resources/enums?view=graph-rest-beta#educationuserrole-values) 枚举添加 `faculty` 选项。                              |

### <a name="groups"></a>组
| **更改类型** | **Version** | **说明** |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta | 已将 **assignedlabels** 属性添加到[组](/graph/api/resources/group?view=graph-rest-beta)实体。 此属性表示与组关联的敏感度标签对（标签 ID、标签名称）列表。

### <a name="identity-and-access-azure-ad--identity-protection"></a>身份和访问（Azure AD）| 身份保护

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 添加了 [riskyUserHistoryItem](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta) 实体。 |
| 添加 | Beta | 添加了[列表历史记录](/graph/api/riskyuser-list-history?view=graph-rest-beta)操作。 |

### <a name="mail-outlook"></a>邮件 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | v1.0 | 已添加 [mailSearchFolder](/graph/api/resources/mailsearchfolder?graph-rest-1.0) 实体，该实体从 [mailFolder](/graph/api/resources/mailfolder?graph-rest-1.0) 实体衍生而来并且支持 mailFolder 实体方法。 |

### <a name="reports--office-365-usage-reports"></a>报告 | Office 365 使用率报告

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | Beta  | 向 [oneDriveUsageAccountDetail](/graph/api/resources/oneDriveUsageAccountDetail?view=graph-rest-beta) 实体添加了 **ownerPrincipalName** 属性。|
| 添加        | Beta  | 向 [sharePointSiteUsageDetail](/graph/api/resources/sharePointSiteUsageDetail?view=graph-rest-beta) 实体添加了 **ownerPrincipalName** 属性。|

### <a name="security"></a>安全性

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0       | 向[安全 API](/graph/api/resources/securescore-api-overview?view=graph-rest-1.0) 添加了安全功能分数 API，包括以下资源和操作：<br/>[secureScore](/graph/api/resources/securescore?view=graph-rest-1.0)（及相关实体）<br/>[列出 secureScores](/graph/api/securescores-list?view=graph-rest-1.0)<br/>[secureScoreControlProfile](/graph/api/resources/securescorecontrolprofile?view=graph-rest-1.0)<br/>[列出 secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-list?view=graph-rest-1.0)<br/>[更新 secureScoreControlProfile](/graph/api/securescorecontrolprofiles-update?view=graph-rest-1.0) |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | Beta        | 向 **chatMessageImportance** 枚举添加了 **urgent** 属性。|
| 新增        | Beta        | 向 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 实体添加了 **hostedContents** 导航属性。|
| 添加项        | Beta        | 添加了 **chatMessageHostedContent** 实体来表示由 Microsoft Teams 托管的与 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 关联的内容。 |


## <a name="april-2019"></a>2019 年 4 月

### <a name="change-notifications-webhooks"></a>更改通知（Webhook）

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 添加 `subscriptionRemoved` 和 `missed` 这两种类型的生命周期通知，它们可对 Outlook 资源使用。 订阅应用可执行适当的操作来缓解通知中断的问题。 有关更多详细信息，请参阅[减少 Outlook 资源丢失的订阅和通知](webhooks-outlook-authz.md)。|

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|添加的新实体：<br/>[androidDeviceOwnerCompliancePolicy](/graph/api/resources/intune-deviceconfig-androiddeviceownercompliancepolicy?view=graph-rest-beta)<br/><br/>[macOSExtensionsConfiguration](/graph/api/resources/intune-deviceconfig-macosextensionsconfiguration?view=graph-rest-beta)<br/><br/>[mobileAppDependency](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta)<br/><br/>[mobileAppRelationship](/graph/api/resources/intune-apps-mobileapprelationship?view=graph-rest-beta)<br/><br/>|
|Addition|beta|新增了复杂类型：<br/>[macOSKernelExtension](/graph/api/resources/intune-deviceconfig-macoskernelextension?view=graph-rest-beta)<br/><br/>[macOSLaunchItem](/graph/api/resources/intune-deviceconfig-macoslaunchitem?view=graph-rest-beta)<br/><br/>[mobileAppRelationshipState](/graph/api/resources/intune-apps-mobileapprelationshipstate?view=graph-rest-beta)<br/><br/>[win32LobAppFileSystemRequirement](/graph/api/resources/intune-apps-win32lobappfilesystemrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppPowerShellScriptRequirement](/graph/api/resources/intune-apps-win32lobapppowershellscriptrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppRegistryRequirement](/graph/api/resources/intune-apps-win32lobappregistryrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppRequirement](/graph/api/resources/intune-apps-win32lobapprequirement?view=graph-rest-beta)<br/><br/>|
|Addition|beta 版本|添加的新枚举类型：<br/>[androidDeviceOwnerPlayStoreMode](/graph/api/resources/intune-deviceconfig-androiddeviceownerplaystoremode?view=graph-rest-beta)<br/><br/>[mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta)<br/><br/>[win32LobAppPowerShellScriptDetectionType](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetectiontype?view=graph-rest-beta)<br/><br/>|
|Addition|beta|添加了 [updateRelationships](/graph/api/intune-apps-mobileapp-updaterelationships?view=graph-rest-beta)<br/> 操作（针对 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)）<br/> |
|添加项|beta|针对 [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta) 集合添加了**导入**<br/> 操作 |
|添加|beta|针对 [mobileApp](/graph/api/intune-apps-mobileapp-getrelatedappstates?view=graph-rest-beta) 添加了 [getRelatedAppStates](/graph/api/intune-apps-mobileapp-getrelatedappstates?view=graph-rest-beta)<br/>  函数<br/> |
|添加项|beta|向 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **kioskModeBluetoothConfigurationEnabled**、**kioskModeWiFiConfigurationEnabled**、**passwordMinimumLetterCharacters**、**passwordMinimumLowerCaseCharacters**、**passwordMinimumNonLetterCharacters**、**passwordMinimumNumericCharacters**、**passwordMinimumSymbolCharacters**、**passwordMinimumUpperCaseCharacters** 和 **playStoreMode**<br/> 属性|
|添加项|beta|向 [androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameType**<br/> 属性|
|删除|beta|从 [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) 实体中删除了 **subjectAlternativeNameType**<br/> 属性|
|删除|beta|从 [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) 实体中删除了 **subjectAlternativeNameType**<br/> 属性|
|添加项|beta|向 [androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameType**<br/> 属性|
|删除|beta|从 [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta) 实体中删除了 **subjectAlternativeNameType**<br/> 属性|
|删除|beta|从 [androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta) 实体中删除了 **subjectAlternativeNameType**ss<br/> 属性|
|添加项|beta|向 [depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta) 实体添加了 **deviceNameTemplate**<br/> 属性|
|添加项|beta|向 [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **importId**<br/> 属性|
|添加项|beta|向 [macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta) 实体添加了 **autoLaunchItems**、**adminShowHostInfo**、**loginWindowText**、**authorizedUsersListHidden**、**authorizedUsersListHideLocalUsers**、**authorizedUsersListHideMobileAccounts**、**authorizedUsersListIncludeNetworkUsers**、**authorizedUsersListHideAdminUsers**、**authorizedUsersListShowOtherManagedUsers**、**shutDownDisabled**、**restartDisabled**、**sleepDisabled**、**consoleAccessDisabled**、**shutDownDisabledWhileLoggedIn**、**restartDisabledWhileLoggedIn**、**powerOffDisabledWhileLoggedIn**、**logOutDisabledWhileLoggedIn** 和 **screenLockDisableImmediate**<br/> 属性|
|添加项|beta|向 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 实体添加了 **dependentAppCount**<br/> 属性|
|添加项|beta|向 [win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta) 实体添加了 **requirementRules**<br/> 属性|
|删除|beta|从 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 实体中删除了 **tpmRequired**<br/> 属性|
|添加项|beta|向 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **groupTag**<br/> 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **users** 导航属性<br/> 属性|
|添加项|beta|向 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 实体添加了 **relationships** 导航属性<br/> 属性|
|添加项|beta|向 [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) 复杂类型添加了 **customPrivacyMessage**<br/> 属性|
|添加项|beta|向 [resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta) 枚举类型添加了 **dependencyFailedToInstall**、**dependencyWithRequirementsNotMet**、**dependencyPendingReboot****dependencyWithAutoInstallDisabled**、**autoInstallDisabled**、**installingDependencies**、**powerShellScriptRequirementNotMet**、**registryRequirementNotMet** 和 **fileSystemRequirementNotMet**<br/> 成员|
|添加项|beta|向 [win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta) 枚举类型添加了 **doesNotExist**<br/> 成员|

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|添加|beta|添加的新实体：<br/>[deviceManagementAbstractComplexSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementAbstractComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance?view=graph-rest-beta)<br/>[deviceManagementBooleanSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementbooleansettinginstance?view=graph-rest-beta)<br/>[deviceManagementCollectionSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementcollectionsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementCollectionSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementcollectionsettinginstance?view=graph-rest-beta)<br/>[deviceManagementComplexSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementcomplexsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementcomplexsettinginstance?view=graph-rest-beta)<br/>[deviceManagementIntegerSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementintegersettinginstance?view=graph-rest-beta)<br/>[deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta)<br/>[deviceManagementIntentAssignment](/graph/api/resources/intune-deviceintent-devicemanagementintentassignment?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceSettingStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceState](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicestate?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicestatesummary?view=graph-rest-beta)<br/>[deviceManagementIntentSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementintentsettingcategory?view=graph-rest-beta)<br/>[deviceManagementIntentUserState](/graph/api/resources/intune-deviceintent-devicemanagementintentuserstate?view=graph-rest-beta)<br/>[deviceManagementIntentUserStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentuserstatesummary?view=graph-rest-beta)<br/>[deviceManagementSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementsettingcategory?view=graph-rest-beta)<br/>[deviceManagementSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementsettinginstance?view=graph-rest-beta)<br/>[deviceManagementStringSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementstringsettinginstance?view=graph-rest-beta)<br/>[deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)<br/>[deviceManagementTemplateSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementtemplatesettingcategory?view=graph-rest-beta)<br/>[securityBaselineDeviceState](/graph/api/resources/intune-deviceintent-securitybaselinedevicestate?view=graph-rest-beta)<br/>[securityBaselineSettingState](/graph/api/resources/intune-deviceintent-securitybaselinesettingstate?view=graph-rest-beta)<br/>[securityBaselineState](/graph/api/resources/intune-deviceintent-securitybaselinestate?view=graph-rest-beta)<br/>[securityBaselineStateSummary](/graph/api/resources/intune-deviceintent-securitybaselinestatesummary?view=graph-rest-beta)<br/>[securityBaselineTemplate](/graph/api/resources/intune-deviceintent-securitybaselinetemplate?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[deviceManagementConstraint](/graph/api/resources/intune-deviceintent-devicemanagementconstraint?view=graph-rest-beta)<br/>[deviceManagementEnumConstraint](/graph/api/resources/intune-deviceintent-devicemanagementenumconstraint?view=graph-rest-beta)<br/>[deviceManagementEnumValue](/graph/api/resources/intune-deviceintent-devicemanagementenumvalue?view=graph-rest-beta)<br/>[deviceManagementSettingBooleanConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingbooleanconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingDependency](/graph/api/resources/intune-deviceintent-devicemanagementsettingdependency?view=graph-rest-beta)<br/>[deviceManagementSettingIntegerConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingintegerconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingRegexConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingregexconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingStringLengthConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingstringlengthconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingXmlConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingxmlconstraint?view=graph-rest-beta)<br/>|
|添加项|beta 版本|添加的新枚举类型：<br/>[deviceManangementIntentValueType](/graph/api/resources/intune-deviceintent-devicemanangementintentvaluetype?view=graph-rest-beta)<br/>[securityBaselineComplianceState](/graph/api/resources/intune-deviceintent-securitybaselinecompliancestate?view=graph-rest-beta)<br/>|
|添加项|beta|在 [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) 上添加了 [createInstance](/graph/api/intune-deviceintent-devicemanagementtemplate-createinstance?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) 上添加了 [updateSettings](/graph/api/intune-deviceintent-devicemanagementintent-updatesettings?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-deviceintent-devicemanagementintent-assign?view=graph-rest-beta) 操作 |
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **intents**、**settingDefinitions**、**templates** 和 **categories** 导航属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **securityBaselineStates** 导航属性|

### <a name="files-sites-and-lists-onedrive-for-business-and-sharepoint"></a>文件、站点和列表（OneDrive for Business 和 SharePoint）

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 添加了 **analytics** 属性至 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 实体。 |
| 添加项        | v1.0        | 添加了 **analytics** 属性至 [site](/graph/api/resources/site?view=graph-rest-beta) 实体。 |
| 添加项        | v1.0        | 添加了 **analytics** 属性至 [listItem](/graph/api/resources/listitem?view=graph-rest-beta) 实体。 |
| 添加项        | v1.0        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 实体上添加了 **getActivitiesByInterval** 函数。 |
| 添加项        | v1.0        | 在 [site](/graph/api/resources/site?view=graph-rest-beta) 实体上添加了 **getActivitiesByInterval** 函数。 |
| 添加项        | v1.0        | 在 [listItem](/graph/api/resources/listitem?view=graph-rest-beta) 实体上添加了 **getActivitiesByInterval** 函数。 |
| 添加项        | v1.0        | 添加了 [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta) 实体。 |
| 添加项        | v1.0        | 添加了 [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta) 实体。 |
| 添加项        | v1.0        | 添加了 [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta) 复杂类型。 |
| 添加项        | v1.0        | 添加了 [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta) 复杂类型。 |
| 添加项        | v1.0        | 添加了 [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta) 复杂类型。 |
| 添加项        | v1.0        | 添加了 **access** 属性至 [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) 复杂类型。 |
| 添加项        | v1.0        | 添加了 **location** 属性至 [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) 复杂类型。 |

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | v1.0 |  为 Azure AD 引入了新的**审核日志 API**，通过 [directoryAudit](/graph/api/resources/directoryAudit?view=graph-rest-1.0) 对目录管理任务提供活动日志，通过 [signIns](/graph/api/resources/signIns?view=graph-rest-1.0) 提供登录活动。。|
| 添加项 | beta | 为**访问评审** API 添加了新的应用程序权限：AccessReview.Read.All、ProgramControl.Read.All 和 ProgramControl.ReadWrite.All。 有关详细信息，请参阅[访问评审 API 参考](/graph/api/resources/accessreviews-root?view=graph-rest-beta)。 |
| 添加项 | beta | 对[用户](/graph/api/resources/user?view=graph-rest-beta)资源添加 **signInSessionsValidFromDateTime** 属性。 这是 **refreshTokensValidFromDateTime** 属性的重命名，但两个属性将均受支持，以使客户端顺畅迁移。 将在接下来的几个月中删除 **refreshTokensValidFromDateTime** 属性。|
| 添加项 | beta | 对[用户](/graph/api/resources/user?view=graph-rest-beta)资源添加 **revokeSignInSessions** 操作。 这是 **invalidateAllRefreshTokens** 属性的重命名，但两项服务操作将均受支持，以使客户端顺畅迁移。 将在接下来的几个月中删除旧的服务操作 **invalidateAllRefreshTokens**。 |
| 添加 | Beta |引入了新的资源类型[trustFrameworkPolicy](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)以支持[Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/active-directory-b2c-overview)。 此资源类型支持[创建](/graph/api/trustframework-post-trustframeworkpolicy?view=graph-rest-beta)、[列表](/graph/api/trustframework-list-trustframeworkpolicies?view=graph-rest-beta)、[获取](/graph/api/trustframeworkpolicy-get?view=graph-rest-beta)、[更新](/graph/api/trustframework-put-trustframeworkpolicy?view=graph-rest-beta)和[删除](/graph/api/trustframerkpolicy-delete?view=graph-rest-beta)操作。|

### <a name="mail-outlook"></a>邮件 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | Beta          | 添加了对 [List Messages](/graph/api/user-list-messages?view=graph-rest-beta) 和 [Get Message](/graph/api/message-get?view=graph-rest-beta) 的新 [Mail.ReadBasic（预览版）权限](permissions-reference.md#mail-permissions)的支持。            |
| 添加        | Beta          | 添加了[获取消息的 MIME 内容](outlook-get-mime-message.md)的功能。 |
| 添加        | Beta          | 向事件、消息、Outlook 任务或组帖子添加了[获取文件或项目附件的原始内容](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment)的功能。 |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 |v1.0 | 增加了对 [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0) 资源的应用程序权限的支持。|
|添加项 |v1.0| 向 [channel](/graph/api/resources/channel?view=graph-rest-1.0) 添加了**email** 和 **webUrl** 属性。|
|添加项 | beta | 添加了 [chat](/api-reference/beta/resources/chat.md) 资源及相关方法。 |
|添加项 |beta| 添加了 API 以读取邮件中的[图像](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)。|
|添加项 | beta | 添加了[对话成员](/api-reference/beta/resources/conversationmember.md) 资源及相关方法。 |


## <a name="march-2019"></a>2019 年 3 月

### <a name="calendar-outlook"></a>日历 (Outlook)
| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 | v1.0 | 添加了 [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) 操作，以及 [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-1.0)、[scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-1.0) 和 [scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-1.0) 复杂类型，来支持[获取给定时间内用户的空闲/忙碌、可用性信息、通讯组列表和资源](outlook-get-free-busy-schedule.md)。 |
|更改 | Beta 版本 | 已回滚到与 [2019 年 2 月](#february-2019)记录的 [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta) 相关的类型更改。 以下行中列出了具体更改内容。|
|更改 | Beta 版本 | 更改了 [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta) 的以下参数的数据类型： <br>**attendees**：从 **attendeeDataModel** 改回为 [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-beta) <br>**locationConstraint**：从 **locationConstraints** 改回为 [locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-beta) <br> **timeConstraint**：从 **findMeetingTimesTimeConstraints** 改回为 [timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-beta)|
|更改 | Beta 版本 | 将 **findMeetingTimes** 的返回类型从 **findMeetingTimesResponse** 改回为 [meetingTimeSuggestionsResult](/graph/api/resources/meetingTimeSuggestionsResult?view=graph-rest-beta) |
|更改 | Beta 版本 | 将 [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) 的基类型从 **locationDataModel** 改回为 [location](/graph/api/resources/location?view=graph-rest-beta) |
|更改 | Beta 版本 | 更改了 [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) 的以下属性的数据类型： <br> **attendeeAvailability**：从 **attendeeAvailabilityDataModel** 集合改回为 [attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-beta) 集合 <br> **locations**：从 **locationDataModel** 集合改回为 [location](/graph/api/resources/location?view=graph-rest-beta) 集合 <br> **meetingTimeSlot**：从 **meetingTimeSlotDataModel** 改回为 [timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta) <br> **organizerAvailability**：从 **availabilityStatus** 改回为 **freeBusyStatus** |
|删除 | Beta | 复杂类型： <br> **attendeeAvailabilityDataModel** <br> **attendeeDataModel** <br> **findMeetingTimesResponse** <br> **findMeetingTimesTimeConstraints** <br> **locationConstraints** <br> **meetingTimeSlotDataModel** <br> **searchWindowTimeSlot**|
|删除 | Beta | 枚举： <br> **addressType** <br> **availabilityStatus** |
|新增 | Beta | 还原了以下复杂类型： <br> [attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-beta) <br> [locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-beta) <br> [meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-beta) <br>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-beta) |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|添加的新实体：<br/>[windowsHealthMonitoringConfiguration](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringconfiguration?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[windowsFirewallRule](/graph/api/resources/intune-deviceconfig-windowsfirewallrule?view=graph-rest-beta)<br/>|
|添加项|beta 版本|添加的新枚举类型：<br/>[androidManagedAppSafetyNetAppsVerificationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetappsverificationtype?view=graph-rest-beta)<br/>[androidManagedAppSafetyNetDeviceAttestationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype?view=graph-rest-beta)<br/>[windowsAutopilotDeviceType](/graph/api/resources/intune-enrollment-windowsautopilotdevicetype?view=graph-rest-beta)<br/>[windowsFirewallRuleInterfaceTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallruleinterfacetypes?view=graph-rest-beta)<br/>[windowsFirewallRuleNetworkProfileTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes?view=graph-rest-beta)<br/>[windowsFirewallRuleTrafficDirectionType](/graph/api/resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype?view=graph-rest-beta)<br/>[windowsHealthMonitoringScope](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringscope?view=graph-rest-beta)<br/>[windowsUpdateNotificationDisplayOption](/graph/api/resources/intune-deviceconfig-windowsupdatenotificationdisplayoption?view=graph-rest-beta)<br/>|
|添加项|beta|在 [importedDeviceIdentity](/graph/api/resources/intune-enrollment-importeddeviceidentity?view=graph-rest-beta) 集合上添加了 [searchExistingIdentities](o:searchExistingIdentities:Collection(microsoft.graph.importedDeviceIdentity)) 操作 |
|添加项|beta|在 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 上添加了 [assignResourceAccountToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice?view=graph-rest-beta) 操作 |
|添加项|beta|在 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 上添加了 [unassignResourceAccountFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice?view=graph-rest-beta) 操作 |
|删除|beta|删除了以下枚举类型：<br/>**defenderScheduleScanDay**<br/>|
|添加项|beta|向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **requiredAndroidSafetyNetDeviceAttestationType**、**appActionIfAndroidSafetyNetDeviceAttestationFailed**、**requiredAndroidSafetyNetAppsVerificationType** 和 **appActionIfAndroidSafetyNetAppsVerificationFailed** 属性|
|添加项|beta|向 [androidManagedStoreApp](/graph/api/resources/intune-apps-androidmanagedstoreapp?view=graph-rest-beta) 实体添加了 **supportsOemConfig** 属性|
|添加项|beta|向 [androidManagedStoreAppConfiguration](/graph/api/resources/intune-apps-androidmanagedstoreappconfiguration?view=graph-rest-beta) 实体添加了 **appSupportsOemConfig** 属性|
|添加项|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **requiredAndroidSafetyNetDeviceAttestationType**、**appActionIfAndroidSafetyNetDeviceAttestationFailed**、**requiredAndroidSafetyNetAppsVerificationType** 和 **appActionIfAndroidSafetyNetAppsVerificationFailed** 属性|
|添加项|beta|向 [depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta) 实体添加了 **iCloudStorageDisabled** 和 **chooseYourLockScreenDisabled** 属性|
|添加项|beta|向 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|Addition|beta|向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体添加了 **allowedOutboundClipboardSharingExceptionLength** 属性|
|添加项|beta|向 [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) 实体添加了 **fastFirstSignIn** 属性|
|添加项|beta|向 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 属性添加了 **tpmRequired** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **firewallRules** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **authenticationWebSignIn**、**privacyDisableLaunchExperience** 和 **appManagementPackageFamilyNamesToLaunchAfterLogOn** 属性|
|删除|beta|从 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体中删除了 **defenderScheduleScanDay** 属性|
|添加项|beta|向 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 实体添加了 **deviceType** 属性|
|添加项|beta|向 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **resourceName**、**skuNumber**、**systemFamily**、**azureActiveDirectoryDeviceId** 和 **managedDeviceId** 属性|
|删除|beta|从 [windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta) 实体删除了 **edgeKioskResetAfterIdleTimeInMinutes** 属性|
|添加项|beta|向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **userWindowsUpdateScanAccess** 和 **updateNotificationLevel** 属性|
|添加项|beta|向 [excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta) 复杂类型添加了 **teams** 属性|
|添加项|beta 版本|向 [windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta) 复杂类型添加了 **autoLaunch** 属性|
|添加项|beta 版本|向 [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) 复杂类型添加了 **allowAccessToDownloadsFolder** 属性|
|添加项|beta 版本|向 [androidDeviceOwnerRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype?view=graph-rest-beta) 枚举类型添加了 **lowSecurityBiometric** 成员|
|添加项|beta 版本|向 [managedAppFlaggedReason](/graph/api/resources/intune-mam-managedappflaggedreason?view=graph-rest-beta) 枚举类型添加了 **androidBootloaderUnlocked** 和 **androidFactoryRomModified** 成员|

### <a name="education"></a>教育
| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta 版本 | 添加新的 [educationCategory](/graph/api/resources/educationCategory?view=graph-rest-beta) 资源。|
| 添加项 | beta 版本 | 添加 API，以在 [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta) 和 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta) 上管理 [educationCategory](/graph/api/resources/educationCategory?view=graph-rest-beta) 资源。|
| 添加项 | beta 版本 | 添加新的 [educationFormResource](/graph/api/resources/educationFormResource?view=graph-rest-beta) 资源。|
| 添加项 | beta 版本 | 在 [educationAssignmentIndividualRecipient](/graph/api/resources/educationAssignmentIndividualRecipient?view=graph-rest-beta) 资源上添加 **recipients** 属性。|

### <a name="files-onedrive-for-business"></a>文件 (OneDrive for Business)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 向 [driveItem](/graph/api/resources/driveItem?view=graph-rest-1.0) 实体添加了 **subscriptions** 导航属性 |
| 添加项        | Beta        | 向 [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) DateTimeOffset 类型添加了 **expirationDateTime** 属性。 |
| 添加项        | Beta        | 向[driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) 字符串类型添加了 **password** 属性。 |

### <a name="financials-dynamics-365-business-central"></a>财务 (Dynamics 365 Business Central)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | beta          | 为 Dynamics 365 Business Central 添加了财务 API。 有关详细信息，请参阅[财务 API 参考](/graph/api/resources/dynamics-graph-reference?view=graph-rest-1.0)。|

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | v1.0 | 在 [domain](/graph/api/resources/domain?view=graph-rest-1.0) 资源上添加 **passwordNotificationWindowInDays** 和 **passwordValidityPeriodInDays** 属性。|
| 添加项 | Beta 和 v1.0 | 添加[设备](/graph/api/resources/device?view=graph-rest-1.0)资源上的 **complianceExpirationDateTime**、**profileType** 和 **systemLabels** 属性。|
| 添加项 | Beta 和 v1.0 | 添加[用户](/graph/api/resources/user?view=graph-rest-1.0)资源上的 **isResourceAccount** 属性。|

### <a name="identity-and-access--identity-protection"></a>身份和访问 | 身份保护

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 |beta 版本| 引入了[“确认风险用户信息已被盗用”](/graph/api/resources/riskyusers-confirmcompromised?view=graph-rest-beta)方法，此方法支持管理员在 Azure AD Identity Protection 中确认用户为已被盗用的用户。 |
|添加项 |beta 版本| 引入了[“删除危险用户”](/graph/api/resources/riskyusers-dismiss?view=graph-rest-beta)方法，此方法支持管理员在 Azure AD Identity Protection 中删除已被标记为存在风险的用户。 |
|添加项 |beta| 向 [riskyUser](/graph/api/resources/riskyuser?view=graph-rest-beta) 资源引入了 **isProcessing** 属性。 |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|删除 |beta| 已从 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 删除 **deleted** 属性。 改用 **deletedDateTime**。 |
| 添加项 | beta 版本 | 添加了 [schedule](/api-reference/beta/resources/schedule.md)、[schedulingGroup](/api-reference/beta/resources/schedulinggroup.md)、[shift](/api-reference/beta/resources/shift.md)、[timeOffReason](/api-reference/beta/resources/timeoffreason.md) 和 [timeOff](/api-reference/beta/resources/timeoff.md) 资源和相关方法。 |


## <a name="february-2019"></a>2019 年 2 月

### <a name="calendar-outlook"></a>日历 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|更改 | Beta 版本 | 更改了 [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta) 的以下参数的数据类型： <br>**attendees**：从 **attendeeBase** 更改为 [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br>**locationConstraint**：从 **locationConstraint** 更改为 [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> **timeConstraint**：从 **timeConstraint** 更改为 [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta)|
|更改 | Beta 版本 | 将 **findMeetingTimes** 的返回类型从 **meetingTimeSuggestionsResult** 更改为 [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) |
|更改 | Beta 版本 | 将 **findMeetingTimes** 的响应有效负载更改为排除每个与会者的**类型**，该类型标识与会者是必需、可选还是资源 |
|更改 | Beta | 将 [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) 的基类型从 [location](/graph/api/resources/location?view=graph-rest-beta) 更改为 [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) |
|更改 | Beta 版本 | 更改了 [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) 的以下属性的数据类型： <br> **attendeeAvailability**：从 **attendeeAvailability** 集合更改为 [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) 集合 <br> **locations**：从 [location](/graph/api/resources/location?view=graph-rest-beta) 集合更改为 [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) 集合 <br> **meetingTimeSlot**：从 [timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta) 更改为 [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> **organizerAvailability**：从 **freeBusyStatus** 更改为 **availabilityStatus** |
|添加项 | Beta | 新复杂类型： <br> [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br> [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) <br> [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta) <br> [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> [postalAddress](/graph/api/resources/postaladdress?view=graph-rest-beta) <br> [searchWindowTimeSlot](/graph/api/resources/searchwindowtimeslot?view=graph-rest-beta)|
|添加项 | Beta | 新枚举： <br> **addressType** <br> **availabilityStatus** |
|新增 | Beta | 已将 **order** 属性添加到 [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) |
|删除 | Beta | 删除了以下复杂类型： <br> **attendeeAvailability** <br> **locationConstraint** <br> **meetingTimeSuggestionsResult** <br>**timeConstraint** |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|Addition|beta|增加了新实体：<br/>[androidOmaCpConfiguration](/graph/api/resources/intune-deviceconfig-androidomacpconfiguration?view=graph-rest-beta)<br/>[managedDeviceEncryptionState](/graph/api/resources/intune-deviceconfig-manageddeviceencryptionstate?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[deliveryOptimizationBandwidth](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidth?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthBusinessHoursLimit](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthHoursWithPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthhourswithpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdCustom](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidcustom?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSource](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsource?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSourceOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsourceoptions?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSize](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesize?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizeAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizeabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizePercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizepercentage?view=graph-rest-beta)<br/>[encryptionReportPolicyDetails](/graph/api/resources/intune-deviceconfig-encryptionreportpolicydetails?view=graph-rest-beta)<br/>|
|添加项|beta|增加了新枚举类型：<br/>[advancedBitLockerState](/graph/api/resources/intune-deviceconfig-advancedbitlockerstate?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdOptionsType](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype?view=graph-rest-beta)<br/>[deliveryOptimizationRestrictPeerSelectionByOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions?view=graph-rest-beta)<br/>[deviceTypes](/graph/api/resources/intune-deviceconfig-devicetypes?view=graph-rest-beta)<br/>[edgeKioskModeRestrictionType](/graph/api/resources/intune-deviceconfig-edgekioskmoderestrictiontype?view=graph-rest-beta)<br/>[encryptionReadinessState](/graph/api/resources/intune-deviceconfig-encryptionreadinessstate?view=graph-rest-beta)<br/>[encryptionState](/graph/api/resources/intune-deviceconfig-encryptionstate?view=graph-rest-beta)<br/>|
|添加项|beta|向 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **autoFillForceAuthentication**、**cellularBlockPlanModification**、**classroomForceAutomaticallyJoinClasses**、**classroomForceUnpromptedAppAndDeviceLock**、**esimBlockModification**、**proximityBlockSetupToNewDevice**、**softwareUpdatesEnforcedDelayInDays** 和 **softwareUpdatesForceDelayed** 属性|
|添加项|beta|向 [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **softwareUpdatesEnforcedDelayInDays**、**softwareUpdatesForceDelayed** 和 **contentCachingBlocked** 属性|
|添加项|beta|向 [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta) 实体添加了 **licensingType** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **defenderSecurityCenterDisableClearTpmUI**、**defenderSecurityCenterDisableNotificationAreaUI**、**defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI**、**defenderAdobeReaderLaunchChildProcess** 和 **defenderOfficeCommunicationAppsLaunchChildProcess** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **edgeKioskModeRestriction**、**edgeKioskResetAfterIdleTimeInMinutes**、**defenderScheduleScanEnableLowCpuPriority**、**defenderDisableCatchupQuickScan**、**defenderDisableCatchupFullScan** 和 **edgeBlockSearchEngineCustomization** 属性|
|添加项|beta|向 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 实体添加了 **enableWhiteGlove** 属性|
|添加项|beta|向 [windowsDeliveryOptimizationConfiguration](/graph/api/resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration?view=graph-rest-beta) 属性添加了 **restrictPeerSelectionBy**、**groupIdSource**、**bandwidthMode**、**backgroundDownloadFromHttpDelayInSeconds**、**foregroundDownloadFromHttpDelayInSeconds**、**minimumRamAllowedToPeerInGigabytes**、**minimumDiskSizeAllowedToPeerInGigabytes**、**minimumFileSizeToCacheInMegabytes**、**minimumBatteryPercentageAllowedToUpload**、**modifyCacheLocation**、**maximumCacheAgeInDays**、**maximumCacheSize** 和 **vpnPeerCaching** 属性|
|添加项|beta|向 [windowsInformationProtectionWipeAction](/graph/api/resources/intune-mam-windowsinformationprotectionwipeaction?view=graph-rest-beta) 实体添加了 **lastCheckInDateTime** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **managedDeviceEncryptionStates** 导航属性|
|添加项|beta|向 [configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta) 复杂类型添加了 **endpointProtection** 和 **officeApps** 属性|
|添加项|beta|向 [win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta) 复杂类型添加了 **productName** 和 **publisher** 属性|
|添加项|beta|向 [managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta) 枚举类型添加了 **warn** 成员|

### <a name="education"></a>教育

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 |beta|在 [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta) 上引入了 relatedContacts 新属性。|
|新增 |v1.0|在 [educationUser](/graph/api/resources/educationUser?view=graph-rest-1.0) 上引入了 relatedContacts 新属性。|

### <a name="files-onedrive-for-business"></a>文件 (OneDrive for Business)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向 [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) DateTimeOffset 类型添加了 **expirationDateTime** 属性。 |
| 添加项        | Beta        | 向[driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) 字符串类型添加了 **password** 属性。 |

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | v1.0 | 添加了新资源类型 [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-1.0)。 |
| 添加项 | Beta 和 v1.0 | 在[组织](/graph/api/resources/organization?view=graph-rest-1.0)上添加了 **createdDateTime** 属性。 |
| 更改 | Beta 和 v1.0 | 已将[用户](/graph/api/resources/user?view=graph-rest-1.0)资源上的 **companyName** 属性更新为可写。 |
| 更改 | beta | [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta) 类型现在包含以前可用于不再支持的派生类型的属性。 |
| 删除 | beta | 不再支持并已删除以下派生类型：**targetResourceDevice**、**targetResourceDirectory**、**targetResourceGroup**、**targetResourcePolicy**、**targetResourceRole**、**targetResourceServicePrincipal**、**targetResourceUser** 和 **targetResourceOther**。 |
| 添加项 |beta | 在 [domain](/graph/api/resources/domain?view=graph-rest-beta) 资源上添加 **passwordNotificationWindowInDays** 和 **passwordValidityPeriodInDays** 属性。|

### <a name="notes-onenote"></a>备注 (OneNote)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | Beta 和 v1.0 | 添加了 [getNotebookFromWebUrl](/graph/api/notebook-getnotebookfromweburl?view=graph-rest-1.0) 方法。 |

### <a name="security"></a>安全性

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta       | 向[安全性 API](/graph/api/resources/security-api-overview?view=graph-rest-beta) 添加了威胁智能 (TI) 指示器 API，包括以下资源和操作：<br/>[tiindicator](/graph/api/resources/tiindicator?view=graph-rest-beta)（及相关实体）<br/> [获取 tiIndicator](/graph/api/tiindicator-get?view=graph-rest-beta)<br/>[创建 tiIndicator](/graph/api/tiindicators-post?view=graph-rest-beta)<br/>[列出 tiIndicator](/graph/api/tiindicators-list?view=graph-rest-beta)<br/>[更新 tiIndicator](/graph/api/tiindicator-update?view=graph-rest-beta) <br/>[删除 tiIndicator](/graph/api/tiindicator-delete?view=graph-rest-beta) <br/>[deleteTiIndicators](/graph/api/tiindicator-deletetiindicators?view=graph-rest-beta) <br/>[deleteTiIndicatorsByExternalId](/graph/api/tiindicator-deletetiindicatorsbyexternalid?view=graph-rest-beta) <br/>[submitTiIndicators](/graph/api/tiindicator-submittiindicators?view=graph-rest-beta) <br/>[updateTiIndicators](/graph/api/tiindicator-updatetiindicators?view=graph-rest-beta)|
| 添加项        | Beta       | 向[安全性 API](/graph/api/resources/security-api-overview?view=graph-rest-beta) 添加了安全操作 API，包括以下资源和操作：<br/>[securityAction](/graph/api/resources/securityaction?view=graph-rest-beta)（及相关实体）<br/> [获取 securityAction](/graph/api/securityaction-get?view=graph-rest-beta)<br/>[创建 securityAction](/graph/api/securityactions-post?view=graph-rest-beta)<br/>[列出 securityAction](/graph/api/securityactions-list?view=graph-rest-beta)<br/>[取消 securityAction](/graph/api/securityaction-cancelsecurityaction?view=graph-rest-beta)
| 添加项        | Beta 版本        | 向警报引入了 [historyStates](/graph/api/resources/alerthistorystate?view=graph-rest-beta) 集合这一复杂类型。 </br>添加了 [updateAlerts](/graph/api/alert-updatealerts?view=graph-rest-beta) 功能，以便更新一个请求中的多个警报。 |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加 |Beta 和 v1.0| 向[团队](/graph/api/resources/team?view=graph-rest-1.0)资源添加了 **internalId** 属性。|
|添加项 |Beta 和 v1.0| 已添加对配置 Word、Excel、PowerPoint、PDF 和文档库[选项卡](teams-configuring-builtin-tabs.md)的支持。 |
|添加项 |beta| 引入了[向频道发送消息](/graph/api/channel-post-messages?view=graph-rest-beta) API。 |
|添加项 |beta| 引入了[在频道中回复消息](/graph/api/channel-post-messagereply?view=graph-rest-beta) API。 |
|删除项 |beta| 删除了 POST /teams/{id}/channels/{id}/chatThreads API。 改用[在频道中创建消息](/graph/api/channel-post-chatmessage?view=graph-rest-beta)。 |
|添加项 |beta | 增加了对 [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) 资源的应用程序权限的支持。|


## <a name="january-2019"></a>2019 年 1 月

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|添加了新实体：<br/>[appleVppTokenTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-applevpptokentroubleshootingevent?view=graph-rest-beta)<br/>[appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta)<br/>[windowsUpdateState](/graph/api/resources/intune-deviceconfig-windowsupdatestate?view=graph-rest-beta)<br/>|
|添加项|beta|添加了新复杂类型：<br/>[appLogCollectionDownloadDetails](/graph/api/resources/intune-devices-applogcollectiondownloaddetails?view=graph-rest-beta)<br/>**deviceManagementTroubleshootingErrorDetails**<br/>[deviceManagementTroubleshootingErrorResource](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource?view=graph-rest-beta)<br/>[win32LobAppAssignmentSettings](/graph/api/resources/intune-apps-win32lobappassignmentsettings?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新枚举类型：<br/>[appLogDecryptionAlgorithm](/graph/api/resources/intune-devices-applogdecryptionalgorithm?view=graph-rest-beta)<br/>[appLogUploadState](/graph/api/resources/intune-devices-apploguploadstate?view=graph-rest-beta)<br/>[win32LobAppNotification](/graph/api/resources/intune-apps-win32lobappnotification?view=graph-rest-beta)<br/>[windowsUpdateStatus](/graph/api/resources/intune-deviceconfig-windowsupdatestatus?view=graph-rest-beta)<br/>|
|添加项|beta|在 [appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta) 上添加了 **createDownloadUrl** 操作 |
|删除|beta|删除了以下实体：<br/>**deviceManagementApplicabilityRuleOsEdition**<br/>**deviceManagementApplicabilityRuleOsVersion**<br/>|
|添加项|beta|向 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体添加了 **passwordSignInFailureCountBeforeFactoryReset** 属性|
|添加项|beta|向 [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) 实体添加了 **passwordSignInFailureCountBeforeFactoryReset** 属性|
|添加项|beta|向 [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) 实体添加了 **passwordSignInFailureCountBeforeFactoryReset** 属性|
|删除|beta|从 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 实体删除了 **defaultProfileDisplayName** 属性|
|添加项|beta|向 [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) 实体添加了 **runAs32Bit** 属性|
|添加项|beta|向 [deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta) 实体添加了 **troubleshootingErrorDetails**、**eventName** 和 **additionalInformation** 属性|
|更改|beta|更改了 [macOSCertificateProfileBase](/graph/api/resources/intune-deviceconfig-macoscertificateprofilebase?view=graph-rest-beta) 实体上的以下属性：<br/>将 **subjectAlternativeNameType** 从必需更改为可选<br/>|
|添加项|beta|向 [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) 实体添加了 **certificateStore** 和 **customSubjectAlternativeNames** 属性|
|添加项|beta|向 [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) 实体添加了 **officeConfigurationXml** 属性|
|添加项|beta|向 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 实体添加了 **createdDateTime** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **bitLockerAllowStandardUserEncryption** 属性|
|删除|beta|从 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体删除了 **localSecurityOptionsEnableAdministratorAccount**、**localSecurityOptionsEnableGuestAccount** 和 **lanManagerWorkstationEnableInsecureGuestLogons** 属性|
|添加项|beta|向 [windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta) 实体添加了 **useSecurityKeyForSignin** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **mobileAppTroubleshootingEvents** 导航属性|
|添加项|beta|向 [mobileAppTroubleshootingEvent](/graph/api/resources/intune-devices-mobileapptroubleshootingevent?view=graph-rest-beta) 实体添加了 **appLogCollectionRequests** 导航属性|

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加 |v1.0|为了支持在 Azure AD B2C 租户中配置标识提供者，引入了新的资源类型 [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-1.0) 实体，以及[创建](/graph/api/identityprovider-post-identityproviders?view=graph-rest-1.0)、[列出](/graph/api/identityprovider-list?view=graph-rest-1.0)、[获取](/graph/api/identityprovider-get?view=graph-rest-1.0)、[更新](/graph/api/identityprovider-update?view=graph-rest-1.0)和[删除](/graph/api/identityprovider-delete?view=graph-rest-1.0)操作。|

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | v1.0 | 在[组](/graph/api/group-list-transitivemembers?view=graph-rest-1.0)上添加了 transitiveMembers 新方法。 此方法返回包含嵌套成员的简单成员列表。|
| 添加项 | v1.0 | 在[用户](/graph/api/user-list-transitivemembersof?view=graph-rest-1.0)、[组](/graph/api/group-list-transitivemembersof?view=graph-rest-beta)和[设备](/graph/api/device-list-transitivemembersof?view=graph-rest-1.0)上添加了 transitiveMemberOf 新方法。|
| 添加项 | v1.0 | 向[用户](/graph/api/resources/user?view=graph-rest-1.0)：**employeeId**、**faxNumber**、**onPremisesDistinguishedName**、**showInAddressList** 和 **otherMails** 中添加了新属性。|
| 添加项 | v1.0 | 向 [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-1.0) 复杂类型添加了 **forceChangePasswordNextSignInWithMfa** 属性。|
| 添加项 | v1.0 | 向 [User](/graph/api/resources/user?view=graph-rest-1.0) 实体添加了 **licenseAssignmentStates** 属性以获取[基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。|
| 添加项 | v1.0 | 添加了 **licenseAssignmentState** 资源以获取[基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。|
| 添加项 | v1.0 | 向 [Group](/graph/api/resources/group?view=graph-rest-1.0) 实体添加了 **assignedLicenses**、**licenseProcessingState** 和 **hasMembersWithLicenseErrors** 属性及 **membersWithLicenseErrors** 关系以获取[基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。|
| 添加项 | beta 版本 | 向 [organization](/graph/api/resources/user?view=graph-rest-beta) 实体添加了 **createdDateTime** 属性。|

### <a name="reports"></a>报告

| **更改类型** | **Version** | **说明**                  |
|:----------------|:------------|:-----------------------------------------|
| 添加        | beta  | 已将 **office365Active** 和 **office365Inactive** 属性添加到 [office365ServicesUserCounts](/graph/api/resources/office365ServicesUserCounts?view=graph-rest-beta) 实体。|

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 |beta 版本| 向 [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) 枚举添加了 educationStandard、educationClass、educationProfessionalLearningCommunity、educationStaff 和 unknownFutureValue。|


## <a name="december-2018"></a>2018 年 12 月

### <a name="identity-and-access--data-policy-operation"></a>身份和访问|数据策略操作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|添加项 |v1.0| 添加了新实体 [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-1.0)。 这表示可用于跟踪目的的提交数据策略操作。
|添加项 |v1.0| 在 [users](/graph/api/resources/users?view=graph-rest-1.0) 上添加了 [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-1.0) 操作。 此操作将提交数据策略操作请求，以导出由 Microsoft 为用户存储的个人数据。 |
|添加项 |v1.0| 添加了方法 [dataPolicyOperations](/graph/api/datapolicyoperation-get?view=graph-rest-1.0)。 该方法将检索 dataPolicyOperation 对象的属性。|

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta 版本 | 已将新属性 `expirationDateTime` 添加到 [group expiration](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-lifecycle) 的[组](https://docs.microsoft.com/graph/api/resources/group?view=graph-rest-beta)。|
| 添加项 | beta 版本 | 添加了新资源类型 [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta)。|
| 添加项 | beta | 向 [organization](/graph/api/resources/organization?view=graph-rest-beta) 资源添加了 `createdDateTime` 属性。|
| 添加项 | v1.0 | 添加了 `memberOf` 方法以获取[设备的](/graph/api/resources/device?view=graph-rest-1.0)直接[成员身份](/graph/api/device-list-memberOf?view=graph-rest-1.0)。 添加此方法是为了获取成员身份列表，包括嵌套成员身份。|
| 更改    | Beta | 重新整理了[组织联系人](/graph/api/resources/orgcontact?view=graph-rest-beta)资源。 物理地址属性（`city`、`country`、`postalCode`、`streetAddress` 和 `state`）和 `officeLocation` 现在位于 `addresses` 集合（采用新的 [physicalOfficeAddress](/graph/api/resources/physicalofficeaddress?view=graph-rest-beta) 资源类型），`mobilePhone`、`businessPhones` 和 `faxNumber` 现在位于 `phones` 集合中。 还添加了 `companyName` 和 `imAddresses`|

### <a name="identity-and-access--privileged-identity-management"></a>身份和访问|特权身份管理

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | beta 版本 | 向 [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) 实体添加了 `registeredRoot` 属性。|
| 更改 | beta 版本 | 将 [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) 实体的属性 `onboardDateTime` 重命名为 `registeredDateTime`。|
| 添加项 | beta 版本 | 添加了新操作 [register resource](/graph/api/governanceresource-register?view=graph-rest-beta)。|
| 删除 | beta | 在 [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta) 实体上删除了 `isPermanent` 属性。|
| 删除 | beta | 在 [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) 实体上删除了 `roleAssignmentStartDateTime` 属性。|
| 删除 | beta | 在 [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) 实体上删除了 `roleAssignmentEndDateTime` 属性。|

### <a name="security"></a>安全性

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 引入了新的复杂类型 [complianceInformation](/graph/api/complianceInformation/team?view=graph-rest-beta)。|
| 添加        | Beta        | 引入了新的复杂类型 [certificationControl](/graph/api/certificationControl/team?view=graph-rest-beta)。|

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Addition |beta 版本| 引入了新资源类型 [teamsTemplate](/graph/api/resources/teamstemplate?view=graph-rest-beta)。|
|添加项 |beta 版本| 引入了新资源类型 [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta)。|
|添加项 |beta| 向 [channel](/graph/api/resources/channel?view=graph-rest-beta) 添加了 isFavoriteByDefault、email 和 webUrl 属性。|
|添加项 |beta 版本| 向 [team](/graph/api/resources/team?view=graph-rest-beta) 添加了 displayName 属性。|
|添加项 |beta 版本| 向 [team](/graph/api/resources/team?view=graph-rest-beta) 添加了 description 属性。|
|添加项 |beta 版本| 向 [team](/graph/api/resources/team?view=graph-rest-beta) 添加了 classification 属性。|
|添加项 |beta 版本| 向 [team](/graph/api/resources/team?view=graph-rest-beta) 添加了 [specialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) 属性。|
|添加项 |beta 版本| 向 [team](/graph/api/resources/team?view=graph-rest-beta) 添加了 [visibility](/graph/api/resources/teamvisibilitytype?view=graph-rest-beta) 属性。|
|添加项 |beta 版本| 向 [team](/graph/api/resources/team?view=graph-rest-beta) 添加了 [template](/graph/api/resources/teamstemplate?view=graph-rest-beta) 属性。|
|添加项 |beta 版本| 向 [team](/graph/api/resources/team?view=graph-rest-beta) 添加了所有者集合。|
|添加项 |beta 版本| 向 teamVisibilityType 中引入了新枚举成员 unknownFutureValue。|
|添加项 |beta 版本| 向 giphyRatingType 中引入了新枚举成员 unknownFutureValue。|
|添加项 |beta 版本| 向 teamsAsyncOperationType 中引入了新枚举成员 unknownFutureValue。|
|添加项 |beta 版本| 向 teamsAsyncOperationStatus 中引入了新枚举成员 unknownFutureValue。|
|添加项 |beta 版本| 向 teamsAppDistributionMethod 中引入了新枚举成员 unknownFutureValue。|
|添加项 |beta 版本| 引入了新资源 [/teamsTemplates](/graph/api/resources/teamstemplate?view=graph-rest-beta)。|
|添加项 | v1.0 | 向 [team](/graph/api/resources/team?view=graph-rest-1.0)、[channel](/graph/api/resources/channel?view=graph-rest-1.0) 和 [tab](/graph/api/resources/teamstab?view=graph-rest-1.0) 操作添加了管理员权限支持。 |


## <a name="november-2018"></a>2018 年 11 月

### <a name="identity-and-access--data-policy-operations"></a>身份和访问|数据策略操作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | beta 版本        | 向 [dataPolicyOperation](/graph/api/resources/dataPolicyOperation?view=graph-rest-beta) 添加了新的 **progress** 属性。 这用于指定操作的进度。

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | v1.0 | 向[域](/graph/api/resources/domain?view=graph-rest-1.0)添加了 [forceDelete](/graph/api/domain-forcedelete?view=graph-rest-1.0) 操作。|
| 添加项 | beta 版本 | 在[组](/graph/api/group-list-transitivemembers?view=graph-rest-beta)上添加了 transitiveMembers 新方法。 此方法返回包含嵌套成员的简单成员列表。|
| 添加项 | beta 版本 | 在[用户](/graph/api/user-list-transitivemembersof?view=graph-rest-beta)、[组](/graph/api/group-list-transitivemembersof?view=graph-rest-beta)、[设备](/graph/api/device-list-transitivemembersof?view=graph-rest-beta)和[服务主体](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta)上添加了 transitiveMemberOf 新方法。|
| 添加项 | beta 版本 | 添加了 memberOf 方法以获取设备的直接[成员身份](/graph/api/device-list-members?view=graph-rest-beta)。 添加此方法是为了获取成员身份列表，包括嵌套成员身份。|
| 添加项 | beta 版本 | 向[用户](/graph/api/resources/user?view=graph-rest-beta)添加了新属性：**faxNumber**、**onPremisesDistinguishedName** 和 **otherMails**。|
| 添加项 | beta | 向 [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-beta) 复杂类型添加了 **forceChangePasswordNextSignInWithMfa** 属性。|
| Addition    | beta | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 对象添加了“externalUserState”和“externalUserStateChangeDateTime”属性。|

### <a name="reports"></a>报告

| 更改类型 | 版本                                    | 说明                              |
| :---------- | :----------------------------------------- | :--------------------------------------- |
| 添加项    | 由世纪互联运营的 Microsoft Graph 中国中的 Beta 版本 | 新增了以下 API：<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta)。 |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加 |v1.0| 引入了新资源类型 [team](/graph/api/resources/team?view=graph-rest-1.0)。|
|添加 |v1.0| 引入了新资源类型 [channel](/graph/api/resources/channel?view=graph-rest-1.0)。|
|添加 |v1.0| 引入了新资源类型 [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-1.0)。|
|添加项 |v1.0| 引入了新资源类型 [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-1.0)。|
|添加 |v1.0| 引入了新资源类型 [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0)。|
|添加 |v1.0| 引入了新资源类型 [teamsAsyncOperation](/graph/api/resources/teamsasyncoperation?view=graph-rest-1.0)。 |
|添加 |v1.0| 引入了新复杂类型 [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-1.0)。 |
|添加 |v1.0| 引入了新复杂类型 [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-1.0)。 |
|添加 |v1.0| 引入了新复杂类型 [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-1.0)。 |
|添加 |v1.0| 引入了新复杂类型 [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-1.0)。 |
|添加项 |v1.0| 引入了新操作[克隆团队](/graph/api/team-clone?view=graph-rest-1.0)。 |
|添加项 |v1.0| 引入了新操作[存档团队](/graph/api/team-archive?view=graph-rest-1.0)。|
|添加项 |v1.0| 引入了新操作[接档团队](/graph/api/team-unarchive?view=graph-rest-1.0)。 |
|添加         | Beta          | 添加了对[克隆团队](/graph/api/team-clone?view=graph-rest-beta)的应用程序权限支持。 |
|添加项 |beta 版本| 引入了 [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta)，它将用有效负载上的一些差异来替换 /teams/{id}/apps。 |
|添加项 |beta 版本| 引入了 [/appCatalogs/teamsApps/{id}/appDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta)，它将替换 [/appCatalogs/teamsApps/{id}](/graph/api/resources/teamsapp?view=graph-rest-beta) 上的版本属性。 |
|更改   |beta 版本| 将类型 [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) 从 teamsCatalogApp 重命名为 teamsApp。 |
|更改   |beta 版本| 将 [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) 上的 distributionMethod 属性类型从 teamsCatalogAppDistributionMethod 重命名为 teamsAppDistributionMethod  |
|删除 |beta| teamsCatalogAppDistributionMethod 已重命名为 teamsAppDistributionMethod  |
|添加项 |beta 版本| 引入了 [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta)，它将用有效负载上的一些差异来替换 /teams/{id}/apps。 |
|添加项 |beta 版本| 向 [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) 添加了 displayName 属性 |
|添加项 |beta 版本| 向 [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) 添加了 messageId 属性 |
|添加项 |beta 版本| 向 [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) 添加了 teamsApp 属性 |
|添加项 |beta 版本| 引入了新资源类型 [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta)。|
|添加项 |beta 版本| 引入了新资源类型 [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta)。|
|添加项 |beta 版本| 引入了新资源类型 [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta)。|
|添加项 |beta 版本| 引入了新枚举成员 hiddenMembership to teamVisibilityType。|
|添加项 |beta 版本| 向 teamsAsyncOperationType 引入了新枚举成员 createTeam。|
|添加项 |beta 版本| 引入了新枚举成员 teamsAppDistributionMethod。|
|添加项 |beta 版本| 在 [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) 下引入了新升级应用操作。 |


## <a name="october-2018"></a>2018 年 10 月

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|v1.0|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0) 实体添加了 **tenantLockdownRequireNetworkDuringOutOfBoxExperience** 属性|
|添加项|v1.0|向 [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0) 复杂类型添加了 **v12_0** 属性|
|添加项|beta 版本|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **lastReportAggregationDateTime** 属性|
|添加项|beta 版本|添加了新实体：<br/>[intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)<br/>|
|添加项|beta|添加了新复杂类型：<br/>[deviceAndAppManagementAssignedRoleIds](/graph/api/resources/intune-rbac-deviceandappmanagementassignedroleids?view=graph-rest-beta)<br/>|
|添加项|beta 版本|添加了新枚举类型：<br/>[applicationGuardEnabledOptions](/graph/api/resources/intune-deviceconfig-applicationguardenabledoptions?view=graph-rest-beta)<br/>[autoRestartNotificationDismissalMethod](/graph/api/resources/intune-deviceconfig-autorestartnotificationdismissalmethod?view=graph-rest-beta)<br/>[meteredConnectionLimitType](/graph/api/resources/intune-deviceconfig-meteredconnectionlimittype?view=graph-rest-beta)<br/>|
|添加项|beta 版本|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 上添加了 [enableLegacyPcManagement](/graph/api/intune-deviceconfig-devicemanagement-enablelegacypcmanagement?view=graph-rest-beta) 操作 |
|添加项|beta|在 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 上添加了 [extendFeatureUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause?view=graph-rest-beta) 操作 |
|添加项|beta 版本|在 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 上添加了 [extendQualityUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause?view=graph-rest-beta) 操作 |
|添加项|beta 版本|在 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 上添加了 [unassignUserFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice?view=graph-rest-beta) 操作 |
|添加项|beta 版本|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 上添加了 [getAssignedRoleIdsForLoggedInUser](/graph/api/intune-rbac-devicemanagement-getassignedroleidsforloggedinuser?view=graph-rest-beta) 函数 |
|添加项|beta|在 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 上添加了 [getManagedDevicesWithAppFailures](/graph/api/intune-troubleshooting-user-getmanageddeviceswithappfailures?view=graph-rest-beta) 函数 |
|添加项|beta 版本|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 中添加了 [managedDeviceEnrollmentAbandonmentSummary](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentsummary?view=graph-rest-beta) 函数 |
|添加项|beta 版本|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 中添加了 [managedDeviceEnrollmentAbandonmentDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentdetails?view=graph-rest-beta) 函数 |
|删除|beta|从 [androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta) 实体删除了 **subjectAlternativeNameType** 属性|
|添加项|beta 版本|向 [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameType** 属性|
|添加项|beta 版本|向 [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) 实体添加了 **certificateStore**、**customSubjectAlternativeNames** 和 **subjectAlternativeNameType** 属性|
|删除|beta|从 [androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta) 实体删除了 **subjectAlternativeNameType** 属性|
|Addition|beta 版本|向 [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameType** 属性|
|添加项|beta|向 [androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta) 实体添加了 **certificateStore**、**customSubjectAlternativeNames** 和 **subjectAlternativeNameType** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **legacyPcManangementEnabled** 属性|
|删除项|beta|从 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 属性删除了 **pinRequiredOnLaunchInsteadOfBiometric** 属性|
|添加项|beta 版本|向 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta 版本|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **applicationGuardEnabledOptions** 属性|
|添加项|beta 版本|向 [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) 实体添加了 **selectedMobileAppIds** 属性|
|添加项|beta 版本|向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **engagedRestartDeadlineInDays**、**engagedRestartSnoozeScheduleInDays**、**engagedRestartTransitionScheduleInDays**、**autoRestartNotificationDismissal**、**scheduleRestartWarningInHours** 和 **scheduleImminentRestartWarningInMinutes** 属性|
|添加项|beta 版本|向 [windowsWifiConfiguration](/graph/api/resources/intune-deviceconfig-windowswificonfiguration?view=graph-rest-beta) 实体添加了 **preSharedKey** 和 **meteredConnectionLimit** 属性|
|添加项|beta 版本|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **intuneBrandingProfiles** 导航属性|
|添加项|beta 版本|向 [androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-beta) 复杂类型添加了 **v6_0**、**v7_0**、**v7_1**、**v8_0**、**v8_1** 和 **v9_0** 属性|
|添加项|beta 版本|向 [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta) 复杂类型添加了 **v12_0** 属性|
|删除|beta|从 [win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta) 复杂类型中删除了 **runAsLoggedOnUser** 属性|
|添加项|beta 版本|向 [osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta) 复杂类型添加了 **lastUpdateDateTime** 属性|
|添加项|beta 版本|向 [windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta) 复杂类型添加了 **lastUpdateDateTime** 属性|
|添加项|beta|向 [windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta) 复杂类型添加了 **lastUpdateDateTime** 属性|
|添加项|beta 版本|向 [windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta) 复杂类型添加了 **lastUpdateDateTime** 属性|
|添加项|beta|向 [windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta) 复杂类型添加了 **lastUpdateDateTime** 属性|

### <a name="identity-and-access--audit-logs"></a>标识和访问|审核日志

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|更改   |beta 版本| 将属性 `conditionalAccessPolicies` 重命名为 `appliedConditionalAccessPolicy`。|
|添加项 |beta 版本| 在[登录 API](/graph/api/resources/signin?view=graph-rest-beta) 中引入了其他风险属性，包括 `riskDetail`、`riskLevelAggregated`、`riskLevelDuringSignIn`、`riskEventTypes` 和 `riskState`。|
|添加项 |beta 版本| 在[登录 API](/graph/api/resources/signin?view=graph-rest-beta) 中引入了其他登录属性，包括 `authenticationProcessingDetails`、`originalRequestID`、`isInteractive`、`tokenIssuerName`、`tokenIssuerType`、`correlationId` 和 `processingTimeinMilliseconds`。|
|删除   |beta| 删除了属性 `isRisky`。|

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | beta 版本 | 在[组](/graph/api/group-list-transitivemembers?view=graph-rest-beta)上添加了 transitiveMembers 新方法。 此方法返回包含嵌套成员的简单成员列表。|
| 添加项 | beta 版本 | 在[用户](/graph/api/user-list-transitivemembersof?view=graph-rest-beta)、[组](/graph/api/group-list-transitivemembersof?view=graph-rest-beta)、[设备](/graph/api/device-list-transitivemembersof?view=graph-rest-beta)和[服务主体](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta)上添加了 transitiveMemberOf 新方法。|
| 添加项 | beta 版本 | 添加了 memberOf 方法以获取设备的直接[成员身份](/graph/api/device-list-members?view=graph-rest-beta)。 添加此方法是为了获取成员身份列表，包括嵌套成员身份。|
| 添加项 | beta 版本 | 向[用户](/graph/api/resources/user?view=graph-rest-beta)添加了新属性：**faxNumber**、**onPremisesDistinguishedName** 和 **otherMails**。|
| 添加 | beta | 向 [User](/graph/api/resources/user?view=graph-rest-beta) 实体添加了 **licenseAssignmentStates** 属性以获取[基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。|
| 添加 | beta | 添加了 **licenseAssignmentState** 资源以获取[基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。|
| 添加 | beta | 向 [Group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了 **assignedLicenses**、**licenseProcessingState**、**hasMembersWithLicenseErrors** 和 **membersWithLicenseErrors** 属性以获取[基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。|

### <a name="identity-and-access--identity-protection"></a>身份和访问 | 身份保护

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项 |beta 版本| 引入了 [riskyUsers API](/graph/api/resources/riskyuser?view=graph-rest-beta)，这表示 Azure AD 用户处于危险之中，可以通过 Azure AD Identity Protection 检测到。 |

### <a name="identity-and-access--privileged-identity-management"></a>身份和访问|特权身份管理

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改 | beta 版本 | 更改 [privilegedapproval](/graph/api/resources/privilegedapproval?view=graph-rest-beta) 实体。|
| Addition | beta 版本 | 添加了 [privilegedroleassignmentrequest](/graph/api/resources/privilegedroleassignmentrequest?view=graph-rest-beta) 实体及以下方法和操作：<br> [List](/graph/api/privilegedroleassignmentrequest-list?view=graph-rest-beta) <br> [Create](/graph/api/privilegedroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/privilegedroleassignmentrequest-cancel?view=graph-rest-beta) <br> [My](/graph/api/privilegedroleassignmentrequest-my?view=graph-rest-beta) |
| 添加项 | beta | 为 [privilegedRoleSettings](/graph/api/resources/privilegedrolesettings?view=graph-rest-beta) 添加了 [Update](/graph/api/privilegedrolesettings-update?view=graph-rest-beta)|
| 删除 |beta| 弃用[自激活角色分配](/graph/api/privilegedrole_selfactivate?view=graph-rest-beta)|

### <a name="personal-contacts-outlook"></a>个人联系人 (Outlook)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 删除         | v1.0        | 这是对文档的更正：从 [contact](/graph/api/resources/contact?view=graph-rest-1.0) 实体主题中删除了 **flag** 属性。 该属性从未在 **contact** 实体中可用。|

### <a name="reports"></a>报告
| 更改类型 | 版本 | Description                              |
|:------------|:--------|:-----------------------------------------|
| 添加项    | v1.0    | 向 [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0) 添加了 **Site ID** 属性。 |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项|beta 版本|向[存档团队](/graph/api/team-archive?view=graph-rest-beta)和[解档团队](/graph/api/team-unarchive?view=graph-rest-beta) API 添加了应用程序权限支持。|

### <a name="track-changes"></a>跟踪更改

| **更改类型** | **Version** | **说明**                  |
|:------------|:--------|:-----------------------------------------|
| 添加    | beta   | 为 [directoryObject](/graph/api/directoryobject-delta?view=graph-rest-beta) 添加了 [delta 查询](delta-query-overview.md)功能 |
| 更改      | v1.0 和 beta  | 为[用户](/graph/api/user-delta?view=graph-rest-1.0)和[组](/graph/api/group-delta?view=graph-rest-1.0)返回仅在 JSON 响应中更改的属性的替代行为。 |
| 添加项    | v1.0   | 为 [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) 添加了 [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) 函数，以支持[使用 delta 查询更改跟踪](delta-query-overview.md)。 |


## <a name="september-2018"></a>2018 年 9 月

### <a name="calls-and-online-meetings"></a>呼叫和联机会议

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Change          | Beta 版本        | 更新了[应用程序](/graph/api/resources/application?view=graph-rest-beta)资源，以添加呼叫集合。 |
| 更改          | Beta 版本        | 更新了[操作](/graph/api/resources/operation?view=graph-rest-beta)资源，以支持长时间运行的呼叫和会议 API。 |
| 添加        | Beta        | 添加了[呼叫](/graph/api/resources/call?view=graph-rest-beta)资源，可以管理音频/视频呼叫（起初在 Microsoft Teams 中），包括用于[创建呼叫](/graph/api/application-post-calls?view=graph-rest-beta)、[检索呼叫](/graph/api/call-get?view=graph-rest-beta)、[删除（挂断）呼叫](/graph/api/call-delete?view=graph-rest-beta)、[应答呼叫](/graph/api/call-answer?view=graph-rest-beta)、[拒绝呼叫](/graph/api/call-reject?view=graph-rest-beta)，[重定向呼叫](/graph/api/call-redirect?view=graph-rest-beta)和[转接呼叫](/graph/api/call-transfer?view=graph-rest-beta)的 API。 此外还添加了 API 来支持 [IVR 方案](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)：[播放提示](/graph/api/call-playprompt?view=graph-rest-beta)、[录制呼叫](/graph/api/call-record?view=graph-rest-beta)、[取消媒体处理](/graph/api/call-cancelmediaprocessing?view=graph-rest-beta)和[订阅触摸音通知](/graph/api/call-subscribetotone?view=graph-rest-beta)。 |
| 添加        | beta        | 添加了[参与者](/graph/api/resources/call?view=graph-rest-beta)资源和用于管理音频/视频呼叫以及会议参与者的 API，包括[检索参与者对象](/graph/api/participant-get?view=graph-rest-beta)、[为参与者配置音频混音器](/graph/api/participant-configuremixer?view=graph-rest-beta)、静音[一个](/graph/api/participant-mute?view=graph-rest-beta)或[所有](/graph/api/participant-muteall?view=graph-rest-beta)参与者、[检索呼叫/会议中的参与者列表](/graph/api/call-list-participants?view=graph-rest-beta)以及[邀请参与者](/graph/api/participant-invite?view=graph-rest-beta)加入呼叫/会议。 |
| 添加        | beta        | 为管理和参与呼叫及会议的应用程序添加了 API，包括[共享内容](/graph/api/call-changescreensharingrole?view=graph-rest-beta)、[将本身设置为静音和解除静音](/graph/api/call-unmute?view=graph-rest-beta)，以及[更新与呼叫关联的元数据](/graph/api/call-updatemetadata?view=graph-rest-beta)的功能。 |
| 添加        | beta        | 添加了[音频路由组](/graph/api/resources/audioroutinggroup?view=graph-rest-beta)资源和 API，用于管理多方会话参与者之间的私有音频路由，包括[创建音频路由组](/graph/api/call-post-audioroutinggroups?view=graph-rest-beta)、[检索音频路由组列表](/graph/api/audioroutinggroup-get?view=graph-rest-beta)、[更新](/graph/api/audioroutinggroup-update?view=graph-rest-beta)和[删除](/graph/api/audioroutinggroup-delete?view=graph-rest-beta)。 |
| 添加项        | beta        | 添加了用于管理 Microsoft Teams 在线会议的[在线会议](/graph/api/resources/audioroutinggroup?view=graph-rest-beta)资源和 API。 最初，只有一个用于在线会议的 API，旨在[检索在线会议对象](/graph/api/onlinemeeting-get?view=graph-rest-beta)。 还添加了与会议相关的[音频会议信息](/graph/api/resources/audioconferencing?view=graph-rest-beta)的相关资源（例如，拨号 URL、密码和电话号码）。 |
| 添加        | Beta        | 许多呼叫和会议 API 需要时间来完成，因此为这些长时间运行的操作添加了资源：[特定于呼叫的操作](/graph/api/resources/commsoperation?view=graph-rest-beta)、[播放音频提示](/graph/api/resources/playpromptoperation?view=graph-rest-beta)和[录制](/graph/api/resources/recordoperation?view=graph-rest-beta)。  |

### <a name="data-access-microsoft-graph-data-connect"></a>数据访问（Microsoft Graph 数据连接）

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加项         | 不适用| 引入了批量访问 Office 365 数据的功能。 有关详细信息，请参阅 [Microsoft Graph 数据连接（预览）](data-connect-overview.md)。|

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|新增|v1.0|在 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-1.0) 操作 |
|添加项|beta|添加的新实体：<br/>[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta)<br/>[officeClientConfigurationAssignment](/graph/api/resources/intune-cirrus-officeclientconfigurationassignment?view=graph-rest-beta)<br/>[officeConfiguration](/graph/api/resources/intune-cirrus-officeconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientSecurityConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientsecurityconfiguration?view=graph-rest-beta)<br/>|
|Addition|beta|新增了复杂类型：<br/>[officeClientCheckinStatus](/graph/api/resources/intune-cirrus-officeclientcheckinstatus?view=graph-rest-beta)<br/>[officeConfigurationAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationassignmenttarget?view=graph-rest-beta)<br/>[officeConfigurationGroupAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationgroupassignmenttarget?view=graph-rest-beta)<br/>[officeUserCheckinSummary](/graph/api/resources/intune-cirrus-officeusercheckinsummary?view=graph-rest-beta)<br/>|
|Addition|beta|在 [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-cirrus-officeclientconfiguration-assign?view=graph-rest-beta) 操作 |
|Addition|beta|在 [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) 集合上添加了 **updatePrioritie** 操作 |
|Addition|beta|添加了新实体：<br/>[deviceConfigurationConflictSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationconflictsummary?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)<br/>|
|Addition|beta|添加了新复杂类型：<br/>[deviceConfigurationTargetedUserAndDevice](/graph/api/resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice?view=graph-rest-beta)<br/>[win32LobAppDetection](/graph/api/resources/intune-apps-win32lobappdetection?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetection](/graph/api/resources/intune-apps-win32lobappfilesystemdetection?view=graph-rest-beta)<br/>[win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta)<br/>[win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)<br/>[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)<br/>[win32LobAppProductCodeDetection](/graph/api/resources/intune-apps-win32lobappproductcodedetection?view=graph-rest-beta)<br/>[win32LobAppRegistryDetection](/graph/api/resources/intune-apps-win32lobappregistrydetection?view=graph-rest-beta)<br/>[win32LobAppReturnCode](/graph/api/resources/intune-apps-win32lobappreturncode?view=graph-rest-beta)<br/>[windows10AppsForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windows10appsforceupdateschedule?view=graph-rest-beta)<br/>|
|Addition|beta|添加了新枚举类型：<br/>[administratorConfiguredDeviceComplianceState](/graph/api/resources/intune-deviceconfig-administratorconfigureddevicecompliancestate?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[microsoftStoreForBusinessPortalSelectionOptions](/graph/api/resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions?view=graph-rest-beta)<br/>[win32LobAppDetectionOperator](/graph/api/resources/intune-apps-win32lobappdetectionoperator?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)<br/>[win32LobAppMsiPackageType](/graph/api/resources/intune-apps-win32lobappmsipackagetype?view=graph-rest-beta)<br/>[win32LobAppRegistryDetectionType](/graph/api/resources/intune-apps-win32lobappregistrydetectiontype?view=graph-rest-beta)<br/>[win32LobAppReturnCodeType](/graph/api/resources/intune-apps-win32lobappreturncodetype?view=graph-rest-beta)<br/>[windows10AppsUpdateRecurrence](/graph/api/resources/intune-deviceconfig-windows10appsupdaterecurrence?view=graph-rest-beta)<br/>[windowsAppStartLayoutTileSize](/graph/api/resources/intune-deviceconfig-windowsappstartlayouttilesize?view=graph-rest-beta)<br/>[windowsAutopilotProfileAssignmentDetailedStatus](/graph/api/resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus?view=graph-rest-beta)<br/>|
|Addition|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 添加了 **overrideComplianceState** 操作 |
|Addition|beta|向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 集合添加了 **getTargetedUsersAndDevices** 操作 |
|Addition|beta|在 [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) 上添加了 [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) 函数 |
|Addition|beta|向 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体添加了 **restrictedApps** 属性|
|Addition|beta|向 [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)实体添加了 **tokenCreationDateTime** 属性|
|删除项|beta|从 [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) 实体中删除了 **restrictedApps** 属性|
|删除项|beta|从 [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) 实体中删除了 **restrictedApps** 属性|
|更改|beta|更改了 [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) 实体上的以下属性：<br/>将 **enablePerApp** 从必需更改为可选<br/>|
|添加项|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **disableProtectionOfManagedOutboundOpenInData** 和 **protectInboundDataFromUnknownSources** 属性|
|添加项|beta|向 [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-beta) 实体添加了 **microsoftStoreForBusinessPortalSelection** 属性|
|添加项|beta|向 [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) 实体添加了 **passcodeMinutesOfInactivityBeforeScreenTimeout** 属性|
|添加项|beta|向 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体添加了 **useOAuth** 属性|
|添加项|beta|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **kioskModeBlockVolumeButtons**、**classroomForceRequestPermissionToLeaveClasses**、**keychainBlockCloudSync**、**pkiBlockOTAUpdates**、**privacyForceLimitAdTracking**、**enterpriseBookBlockBackup**、**enterpriseBookBlockMetadataSync**、**airPrintBlocked**、**airPrintBlockCredentialsStorage**、**airPrintForceTrustedTLS**、**airPrintBlockiBeaconDiscovery**、**blockSystemAppRemoval** 和 **vpnBlockCreation** 属性|
|添加项|beta|向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **disableProtectionOfManagedOutboundOpenInData** 和 **protectInboundDataFromUnknownSources** 属性|
|添加项|beta|向 [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) 实体添加了 **gatekeeperAllowedAppSource** 属性|
|添加项|beta|向 [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **keychainBlockCloudSync**、**airPrintBlocked**、**airPrintForceTrustedTLS** 和 **airPrintBlockiBeaconDiscovery** 属性|
|添加项|beta|向 [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) 实体添加了 **deviceModel** 和 **deviceManufacturer** 属性|
|添加项|beta|向 [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) 实体添加了 **enabledForScopeValidation** 属性|
|添加项|beta|向 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) 实体添加了 **claimTokenManagementFromExternalMdm** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **windows10AppsForceUpdateSchedule** 属性|
|添加项|beta|向 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **deploymentProfileAssignmentDetailedStatus** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceConfigurationConflictSummary** 和 **importedWindowsAutopilotDeviceIdentityUploads** 导航属性|
|添加项|beta|向 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **intendedDeploymentProfile** 导航属性|
|添加项|beta|向 [windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta) 复杂类型添加了 **startLayoutTileSize** 和 **name** 属性|
|添加项|beta|向 [windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta) 复杂类型添加了 **desktopApplicationId** 和 **desktopApplicationLinkPath** 属性|
|删除项|beta|从 [windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta) 复杂类型删除了 **name** 属性|
|添加项|beta|向 [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) 复杂类型添加了 **disallowDesktopApps** 属性|
|更改|beta|更改了 [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) 复杂类型上的以下属性：<br/>将 **startMenuLayoutXml** 从必需更改为可选<br/>|
|添加项|beta|向 [windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta) 复杂类型添加了 **v10_1607**、**v10_1703**、**v10_1709** 和 **v10_1803** 属性|
|添加项|beta|向 [androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **paloAltoGlobalProtect** 成员|
|添加项|beta|向 [deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-beta) 枚举类型添加了 **remoteLock** 成员|

### <a name="files-sites-and-lists-onedrive-for-business-and-sharepoint"></a>文件、站点和列表（OneDrive for Business 和 SharePoint）

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 上的 [createUploadSession](/graph/api/driveitem-createuploadsession?view=graph-rest-beta) 操作添加了 **deferCommit** 参数|
| 添加项        | Beta        | 添加了 [storagePlanInformation](/graph/api/resources/storageplaninformation?view=graph-rest-beta) 复杂类型 |
| 添加项        | Beta        | 向 [quota](/graph/api/resources/quota?view=graph-rest-beta) 复杂类型添加了 **storagePlanInformation** 属性 |
| 添加项        | Beta        | 向 [drive](/graph/api/resources/drive?view=graph-rest-beta) 实体添加了 **following** 导航属性 |
| 添加项        | Beta        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 上添加了 [follow](/graph/api/driveitem-follow?view=graph-rest-beta) 操作 |
| 添加项        | Beta        | 向 [permission](/graph/api/resources/permission?view=graph-rest-beta) 实体添加了 **hasPassword** 属性 |
| 添加项        | Beta        | 向 [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta) 复杂类型添加了 **preventsDownload** 属性 |
| 添加项        | Beta        | 向 [sharedDriveItem](/graph/api/resources/shareddriveitem?view=graph-rest-beta) 实体添加了 **permission** 导航属性 |
| 添加项        | Beta        | 向 [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta) 实体添加了 **geolocation** 属性 |
| 添加项        | Beta        | 添加了 [geolocationColumn](/graph/api/resources/geolocationcolumn?view=graph-rest-beta) 复杂类型 |
| 添加项        | Beta        | 向 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 实体添加了 **analytics** 属性 |
| 添加项        | Beta        | 向 [site](/graph/api/resources/site?view=graph-rest-beta) 实体添加了 **analytics** 属性 |
| 添加项        | Beta        | 向 [listItem](/graph/api/resources/listitem?view=graph-rest-beta) 实体添加了 **analytics** 属性 |
| 添加项        | Beta        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 实体上添加了 **getActivitiesByInterval** 函数 |
| 添加项        | Beta        | 在 [site](/graph/api/resources/site?view=graph-rest-beta) 实体上添加了 **getActivitiesByInterval** 函数 |
| 添加项        | Beta        | 在 [listItem](/graph/api/resources/listitem?view=graph-rest-beta) 实体上添加了 **getActivitiesByInterval** 函数 |
| 添加项        | Beta        | 添加了 [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta) 实体 |
| 添加项        | Beta        | 添加了 [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta) 实体 |
| 添加项        | Beta        | 添加了 [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta) 复杂类型 |
| 添加项        | Beta        | 添加了 [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta) 复杂类型 |
| 添加项        | Beta        | 添加了 [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta) 复杂类型 |
| 添加项        | Beta        | 向 [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) 复杂类型添加了 **access** 属性 |
| 添加项        | Beta        | 向 [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) 复杂类型添加了 **location** 属性 |
| 新增        | v1.0        | 在 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 实体上添加了 **preview** 操作 |
| 新增        | v1.0        | 添加了 [itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-1.0) 复杂类型 |

### <a name="financials-dynamics-365-business-central"></a>财务 (Dynamics 365 Business Central)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | Beta          | 为 Dynamics 365 Business Central 添加了财务 API。 有关详细信息，请参阅[财务 API 参考](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)

### <a name="mail-outlook"></a>邮件 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | [message](/graph/api/resources/message?view=graph-rest-1.0) 实体的 **** 属性现在消息创建上可写。 |

### <a name="notifications-project-rome"></a>通知 (Project Rome)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加          | Beta        | 添加了 [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta) 资源类型。 |
| 添加项          | Beta        | 添加了[创建和发布通知](/graph/api/projectrome_notification_post?view=graph-rest-beta) API。|

### <a name="security"></a>安全性

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta       | 向[安全 API](/graph/api/resources/securescore-api-overview?view=graph-rest-beta) 添加了安全功能分数 API，包括以下资源和操作：<br/>[secureScores](/graph/api/resources/securescores?view=graph-rest-beta)（和相关实体）<br/>[列出 secureScores](/graph/api/securescores-list?view=graph-rest-beta)<br/>[secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta)<br/>[列出 secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-list?view=graph-rest-beta)<br/>[更新 secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-update?view=graph-rest-beta) |
| 添加项        | Beta        | 引入了新的复杂类型 [secureScoreControlStateUpdate](/graph/api/resources/securescorecontrolstateupdate?view=graph-rest-beta) |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加|beta|添加了用于[选项卡](/graph/api/resources/teamstab?view=graph-rest-beta)的 API。|
|加|beta|添加了用于[为组织发布应用](/graph/api/resources/teamsapp?view=graph-rest-beta)的 API。|
|加|beta|添加了对 [GET /teams/{id}](/graph/api/team-get?view=graph-rest-beta) 的应用程序权限支持。 |
|加|beta|添加了对 [GET /teams/{id}/channels](/graph/api/group-list-channels?view=graph-rest-beta) 的应用程序权限支持。 |
|添加项|beta|添加了对 [GET /teams/{id}/channels/{id}](/graph/api/channel-get?view=graph-rest-beta) 的应用程序权限支持。 |
|添加项|beta|添加了对 [PUT /groups/{id}/team](/graph/api/team-put-teams?view=graph-rest-beta) 的应用程序权限支持。 |
|添加项|beta|添加了对 [PATCH /teams/{id}](/graph/api/team-update?view=graph-rest-beta) 的应用程序权限支持。 |
|添加项|beta|添加了对[创建通道](/graph/api/channel-post?view=graph-rest-beta)、[更新通道](/graph/api/channel-patch?view=graph-rest-beta)，和[删除通道](/graph/api/channel-delete?view=graph-rest-beta)的应用程序权限支持。 |
|删除项|beta| 从 [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) 删除了 isBlocks 和 installedState 属性。|
|更改| beta | [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) 上的上下文属性已重命名为 distributionMethod。|


## <a name="august-2018"></a>2018 年 8 月

### <a name="calendar-outlook"></a>日历 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 添加了 [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) 操作，以及 [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-beta)、[scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-beta) 和 [scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-beta) 复杂类型，来支持[获取给定时间内用户的空闲/忙碌、可用性信息、通讯组列表和资源](outlook-get-free-busy-schedule.md)。 |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|v1.0|添加的新实体：<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-1.0)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-1.0)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-1.0)<br/>|
|添加项|v1.0|添加的新枚举类型：<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-1.0)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-1.0)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-1.0)<br/>|
|添加项|v1.0|在 [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) 中添加了 [managedDeviceEnrollmentFailureDetails](/graph/api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-1.0) 函数 |
|添加项|v1.0|在 [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) 中添加了 [managedDeviceEnrollmentTopFailures](/graph/api/intune-shared-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-1.0) 函数 |
|新增|v1.0|向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0) 实体添加了 **kioskModeBuiltInAppId** 属性|
|添加项|v1.0|向 [complianceStatus](/graph/api/resources/intune-shared-compliancestatus?view=graph-rest-1.0) 枚举类型添加了 **notAssigned** 成员|
|添加项|v1.0|向 [deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-1.0) 枚举类型添加了 **pushNotification** 成员|
|添加项|v1.0|向 [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-1.0) 枚举类型添加了 **userAbandonment** 成员|
|添加项|v1.0|向 [managedDevicePartnerReportedHealthState](/graph/api/resources/intune-devices-manageddevicepartnerreportedhealthstate?view=graph-rest-1.0) 枚举类型添加了 **compromised** 和 **misconfigured** 成员|
|添加项|v1.0|向 [vppTokenState](/graph/api/resources/intune-onboarding-vpptokenstate?view=graph-rest-1.0) 枚举类型添加了 **assignedToExternalMDM** 成员|
||
|添加项|beta|添加的新实体：<br/>[advancedThreatProtectionOnboardingDeviceSettingState](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate?view=graph-rest-beta)<br/>[advancedThreatProtectionOnboardingStateSummary](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary?view=graph-rest-beta)<br/>[depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)<br/>[depEnrollmentProfile](/graph/api/resources/intune-enrollment-depenrollmentprofile?view=graph-rest-beta)<br/>[depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile?view=graph-rest-beta)<br/>[depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta)<br/>[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta)<br/>[importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta)<br/>[importedAppleDeviceIdentityResult](/graph/api/resources/intune-enrollment-importedappledeviceidentityresult?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta)<br/>[windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta)<br/>|
|添加项|beta|添加了新复杂类型：<br/>[configurationManagerClientHealthState](/graph/api/resources/intune-devices-configurationmanagerclienthealthstate?view=graph-rest-beta)<br/>[customSubjectAlternativeName](/graph/api/resources/intune-deviceconfig-customsubjectalternativename?view=graph-rest-beta)<br/>[deviceManagementUserRightsLocalUserOrGroup](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup?view=graph-rest-beta)<br/>[deviceManagementUserRightsSetting](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightssetting?view=graph-rest-beta)<br/>[managementCertificateWithThumbprint](/graph/api/resources/intune-enrollment-managementcertificatewiththumbprint?view=graph-rest-beta)<br/>[mobileAppSupportedDeviceType](/graph/api/resources/intune-troubleshooting-mobileappsupporteddevicetype?view=graph-rest-beta)<br/>[osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta)<br/>[windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta)<br/>[windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta)<br/>[windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta)<br/>[windowsMalwareOverview](/graph/api/resources/intune-devices-windowsmalwareoverview?view=graph-rest-beta)<br/>[windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新枚举类型：<br/>[configurationManagerClientState](/graph/api/resources/intune-devices-configurationmanagerclientstate?view=graph-rest-beta)<br/>[depTokenType](/graph/api/resources/intune-enrollment-deptokentype?view=graph-rest-beta)<br/>[discoverySource](/graph/api/resources/intune-enrollment-discoverysource?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[iTunesPairingMode](/graph/api/resources/intune-enrollment-itunespairingmode?view=graph-rest-beta)<br/>[lanManagerAuthenticationLevel](/graph/api/resources/intune-deviceconfig-lanmanagerauthenticationlevel?view=graph-rest-beta)<br/>[localSecurityOptionsMinimumSessionSecurity](/graph/api/resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity?view=graph-rest-beta)<br/>[resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)<br/>[vpnProviderType](/graph/api/resources/intune-deviceconfig-vpnprovidertype?view=graph-rest-beta)<br/>[windowsMalwareThreatState](/graph/api/resources/intune-devices-windowsmalwarethreatstate?view=graph-rest-beta)<br/>|
|添加项|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 上添加了 [uploadDepToken](/graph/api/intune-enrollment-deponboardingsetting-uploaddeptoken?view=graph-rest-beta) 操作 |
|添加项|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 上添加了 [syncWithAppleDeviceEnrollmentProgram](/graph/api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram?view=graph-rest-beta) 操作 |
|添加项|beta|在 [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) 上添加了 [setDefaultProfile](/graph/api/intune-enrollment-enrollmentprofile-setdefaultprofile?view=graph-rest-beta) 操作 |
|添加项|beta|在 [importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta) 集合上添加了 **importAppleDeviceIdentityList** 操作 |
|添加项|beta|在 [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) 上添加了 [updateDeviceProfileAssignment](/graph/api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) 操作 |
|添加项|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 上添加了 [shareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice?view=graph-rest-beta) 操作 |
|添加项|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 上添加了 [unshareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice?view=graph-rest-beta) 操作 |
|添加项|beta|在 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 上添加了 [assignUserToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 上添加了 [getRoleScopeTagsByResource](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyresource?view=graph-rest-beta) 函数 |
|添加项|beta|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 上添加了 [getRoleScopeTagsByIds](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyids?view=graph-rest-beta) 函数 |
|添加项|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 集合上添加了 [getEncryptionPublicKey](/graph/api/intune-enrollment-deponboardingsetting-getencryptionpublickey?view=graph-rest-beta) 函数 |
|添加项|beta|在 [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) 上添加了 [exportMobileConfig](/graph/api/intune-enrollment-enrollmentprofile-exportmobileconfig?view=graph-rest-beta) 函数 |
|添加项|beta|在 [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) 上添加了 [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) 函数 |
|删除|beta|删除了 **uploadDepToken** 集合 |
|删除|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 集合上删除了 **syncWithAppleDeviceEnrollmentProgram** 操作 |
|删除|beta|在 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 集合上删除了 **getEncryptionPublicKey** 函数 |
|添加项|beta|向 [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) 实体中添加了 **restrictedApps** 属性|
|添加项|beta|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **vpnAlwaysOnPackageIdentifier** 和 **vpnEnableAlwaysOnLockdownMode** 属性|
|删除项|beta|从 [androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta) 实体删除了 **packageName** 属性|
|添加项|beta|向 [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) 实体添加了 **restrictedApps** 属性|
|添加项|beta|向 [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **vpnAlwaysOnPackageIdentifier** 和 **vpnEnableAlwaysOnLockdownMode** 属性|
|添加项|beta|向 [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) 实体添加了 **optInToDeviceIdSharing** 属性|
|添加项|beta|向 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 实体添加了 **tokenType**、**tokenName**、**syncedDeviceCount**、**defaultProfileDisplayName** 和 **dataSharingConsentGranted** 属性|
|添加项|beta|向 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 和 **supportsScopeTags** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **windowsMalwareOverview** 属性|
|更改|beta|更改了 [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) 实体上的以下属性：<br/>将 **subjectAlternativeNameType** 从必需更改为可选<br/>|
|添加项|beta|向 [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) 实体添加了 **restrictedApps** 属性|
|添加项|beta|向 [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) 实体添加了 **certificateStore** 和 **customSubjectAlternativeNames** 属性|
|添加项|beta|向 [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) 实体添加了 **enforcedSoftwareUpdateDelayInDays** 属性|
|添加项|beta|向 [iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta) 实体添加了 **providerType**、**userDomain**、**strictEnforcement**、**cloudName** 和 **excludeList** 属性|
|添加项|beta|向 [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **safariBlockAutofill**、**cameraBlocked**、**iTunesBlockMusicService**、**spotlightBlockInternetResults**、**keyboardBlockDictation**、**definitionLookupBlocked**、**appleWatchBlockAutoUnlock**、**iTunesBlockFileSharing**、**iCloudBlockDocumentSync**、**iCloudBlockMail**、**iCloudBlockAddressBook**、**iCloudBlockCalendar**、**iCloudBlockReminders**、**iCloudBlockBookmarks**、**iCloudBlockNotes**、**airDropBlocked**、**passwordBlockModification** 和 **passwordBlockFingerprintUnlock** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **roleScopeTagIds**、**windowsActiveMalwareCount**、**windowsRemediatedMalwareCount**、**notes** 和 **configurationManagerClientHealthState** 属性|
|添加项|beta|向 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) 实体添加了 **installStateDetail** 属性|
|添加项|beta|向 [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) 实体添加了 **roleScopeTagIds** 属性|
|添加项|beta|向 [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) 实体添加了 **targetVersion** 和 **updateVersion** 属性|
|添加项|beta|向 [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) 实体添加了 **resource** 属性|
|添加项|beta|向 [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) 实体添加了 **localStorage**、**setPowerPolicies** 和 **signInOnResume** 属性|
|添加项|beta|向 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 属性添加了 **configurationManagerComplianceRequired** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)实体添加了 **userRightsAccessCredentialManagerAsTrustedCaller**、**userRightsAllowAccessFromNetwork**、**userRightsBlockAccessFromNetwork**、**userRightsActAsPartOfTheOperatingSystem**、**userRightsLocalLogOn**、**userRightsBackupData**、**userRightsChangeSystemTime**、**userRightsCreateGlobalObjects**、**userRightsCreatePageFile**、**userRightsCreatePermanentSharedObjects**、**userRightsCreateSymbolicLinks**、**userRightsCreateToken**、**userRightsDebugPrograms**、**userRightsRemoteDesktopServicesLogOn**、**userRightsDelegation**、**userRightsGenerateSecurityAudits**、**userRightsImpersonateClient**、**userRightsIncreaseSchedulingPriority**、**userRightsLoadUnloadDrivers**、**userRightsLockMemory**、**userRightsManageAuditingAndSecurityLogs**、**userRightsManageVolumes**、**userRightsModifyFirmwareEnvironment**、**userRightsModifyObjectLabels**、**userRightsProfileSingleProcess**、**userRightsRemoteShutdown**、**userRightsRestoreData**、**userRightsTakeOwnership**、**userRightsRegisterProcessAsService**、**localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients**、**localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers**、**lanManagerAuthenticationLevel** 和 **lanManagerWorkstationEnableInsecureGuestLogons** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **passwordMinimumAgeInDays**、**tenantLockdownRequireNetworkDuringOutOfBoxExperience** 和 **dataProtectionBlockDirectMemoryAccess** 属性|
|添加项|beta|向 [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) 实体添加了 **extendedKeyUsages** 属性|
|添加项|beta|向 [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) 实体添加了 **enableDnsRegistration** 和 **dnsSuffixes** 属性|
|添加项|beta|向 [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta) 实体添加了 **customSubjectAlternativeNames** 属性|
|添加项|beta|向 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 实体添加了 **extractHardwareHash** 和 **deviceNameTemplate** 属性|
|添加项|beta|向 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **addressableUserName** 和 **userPrincipalName**|
|添加项|beta|向 [windowsDeviceMalwareState](/graph/api/resources/intune-devices-windowsdevicemalwarestate?view=graph-rest-beta) 实体添加了 **threatState** 属性|
|添加项|beta|向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **qualityUpdatesPauseStartDateTime**、**featureUpdatesPauseStartDateTime**、**featureUpdatesRollbackWindowInDays**、**qualityUpdatesWillBeRolledBack**、**featureUpdatesWillBeRolledBack**、**qualityUpdatesRollbackStartDateTime** 和 **featureUpdatesRollbackStartDateTime** 属性|
|添加项|beta|向 [windowsWifiEnterpriseEAPConfiguration](/graph/api/resources/intune-deviceconfig-windowswifienterpriseeapconfiguration?view=graph-rest-beta) 属性添加了 **trustedServerCertificateNames** 属性|
|添加项|beta|向 [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) 实体添加了 **defaultIosEnrollmentProfile**、**defaultMacOsEnrollmentProfile**、**enrollmentProfiles** 和 **importedAppleDeviceIdentities** 导航属性|
|添加项|beta|向 [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta) 实体添加了 **roleScopeTags** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **advancedThreatProtectionOnboardingStateSummary**、**roleScopeTags** 和 **importedWindowsAutopilotDeviceIdentityUploads** 导航属性|
|添加项|beta|向 [mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta) 复杂类型添加了 **supportedDeviceTypes** 属性|
|添加项|beta|向 [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 复杂类型添加了 **hideEscapeLink** 属性|
|添加项|beta|向 [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **zscalerPrivateAccess**、**f5Access2018**、**citrixSso** 和 **paloAltoGlobalProtectV2** 成员|
|添加项|beta|向 [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-beta) 枚举类型添加了 **userAbandonment** 成员|
|添加项|beta|向 [enrollmentState](/graph/api/resources/intune-enrollment-enrollmentstate?view=graph-rest-beta) 枚举类型添加了 **blocked** 成员|
|Addition|beta|向 [managementAgentType](/graph/api/resources/intune-shared-managementagenttype?view=graph-rest-beta) 枚举类型添加了 **microsoft365ManagedMdm** 成员|
|添加项|beta|向 [subjectAlternativeNameType](/graph/api/resources/intune-deviceconfig-subjectalternativenametype?view=graph-rest-beta) 枚举类型添加了 **domainNameService** 成员|
|添加项|beta|向 [wiFiSecurityType](/graph/api/resources/intune-deviceconfig-wifisecuritytype?view=graph-rest-beta) 枚举类型添加了 **wpa2Personal** 和 **wpa2Enterprise** 成员|
|加|beta|向 [windowsMalwareCategory](/graph/api/resources/intune-devices-windowsmalwarecategory?view=graph-rest-beta) 枚举类型添加了 **enterpriseUnwantedSoftware**、**ransom** 和 **hipsRule** 成员|

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | v1.0 | 向 [Organization](/graph/api/resources/organization?view=graph-rest-beta) 资源添加了 isMultipleDataLocationsForServicesEnabled 属性，允许应用确认已为多地理位置功能启用了租户。 向 [user](/graph/api/resources/user?view=graph-rest-beta) 和 [group](/graph/api/resources/group?view=graph-rest-beta) 资源添加了 preferredDataLocation 属性，允许为用户和组设置首选数据位置。|
| 添加项 | v1.0 | 向 [User](/graph/api/resources/user?view=graph-rest-1.0) and [Group](/graph/api/resources/group?view=graph-rest-1.0) 实体添加了 [onPremisesProvisioningErrors](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-1.0) 属性，表示在使用 Microsoft 同步产品（包括 Azure AD Connect、DirSync 和 MIM + 连接器），将本地目录同步到 Azure Active Directory 时发生目录同步错误。|
| 添加项 | v1.0 | 向 [User](/graph/api/resources/user?view=graph-rest-1.0) 实体添加了 [onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-1.0) 属性，其中包含 15 个自定义扩展属性。 对于 onPremisesSyncEnabled 用户，此组属性在本地 Active Directory 中进行管理，并同步到 Azure AD，且为只读。 对于只使用云的用户（其中 onPremisesSyncEnabled 为 false），可以在创建或更新期间设置这些属性。|
|添加项|v1.0|向 [User](/graph/api/resources/user?view=graph-rest-1.0) 实体添加了 **onPremisesDomainName**、**onPremisesSamAccountName** 和 **onPremisesUserPrincipalName** 属性|

### <a name="mail-outlook"></a>邮件 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0        | 添加了对 [getMailTips](/graph/api/user-getmailtips?view=graph-rest-1.0) 操作的支持，可以获取特定收件人的所有邮件提示。 添加了以下资源：[automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-1.0)、[mailTips](/graph/api/resources/mailtips?view=graph-rest-1.0)、[mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-1.0)。 |

### <a name="reports"></a>报告
| 更改类型 | 版本 | 说明                              |
|:------------|:--------|:-----------------------------------------|
| 添加项    | v1.0    | 向 [getoffice365activationsuserdetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0) 添加了**在共享计算机上激活**属性。 |
| 添加项    | v1.0    | 向 [getoffice365activationsusercounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0) 添加了**共享计算机激活**属性。 |

### <a name="security"></a>安全性

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | beta       | 向 [alert](/graph/api/resources/alert?view=graph-rest-beta ) 添加了 **activityGroupName**、**cloudAppStates**、**confidence** 和 **registryKeyStates** 属性。 |
|删除|beta| 从 [alert](/graph/api/resources/alert?view=graph-rest-beta ) 删除了 **activityGroupStates**、**applicationStates**、**malwareWasRunning**、**riskScore** 和 **type** 属性。 |
|更改|beta| 将**批注**类型从 `String` 更改为 `String collection`，将**严重性**类型从 `String` 更改为 [alert](/graph/api/resources/alert?view=graph-rest-beta) 中的 [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) 枚举。 |
| 添加项        | beta       | 添加了以下资源类型： <br/> [cloudAppSecurityState](/graph/api/resources/cloudappsecuritystate?view=graph-rest-beta) <br/> [fileHash](/graph/api/resources/filehash?view=graph-rest-beta) <br/> [registryKeyState](/graph/api/resources/registrykeystate?view=graph-rest-beta) |
|删除|beta| 删除了以下资源类型： <br/> **activityGroupState**  <br/> **applicationSecurityState** |
| 添加项        | beta       | 添加了以下枚举： <br/> [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) <br/> [connectionDirection](/graph/api/resources/connectiondirectionenumtype?view=graph-rest-beta) <br/> [connectionStatus](/graph/api/resources/connectionstatusenumtype?view=graph-rest-beta) <br/> [emailRole](/graph/api/resources/emailroleenumtype?view=graph-rest-beta) <br/> [fileHashType](/graph/api/resources/filehashtypeenumtype?view=graph-rest-beta) <br/> [registryHive](/graph/api/resources/registryhiveenumtype?view=graph-rest-beta)  <br/> [registryOperation](/graph/api/resources/registryoperationenumtype?view=graph-rest-beta) <br/> [registryValueType](/graph/api/resources/registryvaluetypeenumtype?view=graph-rest-beta)|
|删除|beta| 删除了以下枚举类型： <br/> **alertType** <br/> **applicationPermissionsRequired** |
| 添加项        | beta       | 向 [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta ) 添加了 **fileHash** 属性。|
|删除|beta| 从 [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta) 删除了 **authenticodeHash256** 和 **sha256** 属性。 |
| 添加项 | beta | 向 [hostSecurityState](/graph/api/resources/hostsecuritystate?view=graph-rest-beta) 添加了 **os** 属性。|
| 添加项 | beta | 向 [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) 添加了 **category**、**family** 和 **wasRunning** 属性。|
|删除|beta| 从 [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) 删除了 **aliases** 属性。 |
|更改|beta| 将 **malwareWasRunning** 属性从 [alert](/graph/api/resources/alert?view=graph-rest-beta ) 移至 [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta)，并重命名为 **wasRunning**。 |
| 添加项        | beta       | 向 [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ) 添加了 **applicationName**、**destinationDomain**、**direction**、**domainRegisteredDateTime**、**localDnsName**、**natDestinationAddress**、**natDestinationPort**、**natSourceAddress**、**natSourcePort**、**riskScore**、**status** 和 **urlParameters** 属性。|
|更改|beta| 将 [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ) 中的 **uri** 属性更改为 **destinationUrl**。 |
| 添加项        | beta       | 向 [process](/graph/api/resources/process?view=graph-rest-beta ) 添加了 **fileHash** 属性。|
|删除项|beta| 从 [process](/graph/api/resources/process?view=graph-rest-beta ) 删除了 **authenticodeHash256** 和 **sha256** 属性。 |
| 添加项        | beta       | 向 [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta) 添加了 **aadUserId**、**emailRole**、**isVpn** 和 **logonIp** 属性。|
|更改|beta| 将 [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta) 中的 **logonIpAddress** 属性更改为 **logonIp**。 |
| 添加项        | beta       | 向 [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta) 添加了 **wasRunning** 属性。|
|删除项|beta| 从 [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta) 删除了 **name** 属性。 |

### <a name="track-changes"></a>跟踪更改

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 在 Azure AD 中为以下实体添加了 [delta 查询](delta-query-overview.md)功能：<br/>[application](/graph/api/application-delta?view=graph-rest-beta)<br/>[directoryRole](/graph/api/directoryrole-delta?view=graph-rest-beta)<br/>[servicePrincipal](/graph/api/serviceprincipal-delta?view=graph-rest-beta) |


## <a name="july-2018"></a>2018 年 7 月

### <a name="change-notifications-webhooks"></a>更改通知（Webhook）
| 更改类型 | 版本 | 说明                              |
|:------------|:--------|:-----------------------------------------|
| 重大更改 | Beta 和 v1.0 | 将驱动器根项的 [Webhook](/graph/api/resources/webhooks?view=graph-rest-1.0) [最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)缩短至 3 天。 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta 版本        | [application](/graph/api/resources/application?view=graph-rest-beta) 和 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) API 将在预览版 (beta) 中得到更新。 第一个更改集将于 2018 年 7 月 16 日应用。 这些更改包括属性重命名和重构。 在更改完成后，大部分现有属性才可用。 将会添加新属性。 这些更改在发布到 v1.0 之前将先在预览版 (beta) 中发布。 |

### <a name="identity-and-access--synchronization"></a>身份和访问|同步

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加 | Beta | 向 [sychronizationStatus](/graph/api/resources/synchronization-synchronizationstatus?view=graph-rest-beta) 添加了 **progress** 属性，以允许客户端监视同步作业的进度。|

### <a name="personal-contacts-outlook"></a>个人联系人 (Outlook)
| **更改类型** | **Version**   | **说明**                          |
|:--------------- |:------------- |:---------------------------------------- |
|添加 |Beta | 添加了复杂类型 [typedEmailAddress](/graph/api/resources/typedemailaddress?view=graph-rest-beta)。 |
|更改 | Beta 版本 | 已将 [contact](/graph/api/resources/contact?view=graph-rest-beta) 的 **emailAddresses** 属性的类型更改为 **typedEmailAddress** 实例集合。|

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|更改|beta|更新了 [chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 资源|
|添加项|beta|添加了 [Chat attachment](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) 资源类型|
|添加项|beta|添加了 [Chat mention](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) 资源类型|
|添加项|beta|添加了 [Chat reaction](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) 资源类型|
|添加项|beta|添加了[获取所有通道邮件 API](/graph/api/channel-list-messages?view=graph-rest-beta) |
|添加项|beta|添加了[获取通道邮件 API](/graph/api/channel-get-message?view=graph-rest-beta) |
|添加项|beta|添加了[获取所有邮件答复 API](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|添加项|beta|添加了[获取邮件答复 API](/graph/api/channel-get-messagereply?view=graph-rest-beta) |
|添加项|beta|添加了对 [/users/{id}/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta) 的应用程序权限支持 |
|添加项|beta|添加了[获取所有通道邮件 API](/graph/api/channel-list-messages?view=graph-rest-beta) |
|添加项|beta|添加了[获取通道邮件 API](/graph/api/channel-get-message?view=graph-rest-beta) |
|添加项|beta|添加了[获取所有邮件答复 API](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|添加项|beta|添加了[获取邮件答复 API](/graph/api/channel-get-messagereply?view=graph-rest-beta) |
|添加项|beta|添加了 [Chat attachment](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) 资源类型|
|添加项|beta|添加了 [Chat mention](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) 资源类型|
|添加项|beta|添加了 [Chat reaction](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) 资源类型|
|更改|beta|更新了 [chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta)) 资源|
|删除|beta|已删除 DELETE /groups/{id}/team/channels/{id}，请改用 DELETE /teams/{id}/channels/{id}。 |
|删除|beta|已删除 GET /groups/{id}/team/channels/{id}，请改用 GET /teams/{id}/channels/{id}。 |
|删除|beta|已删除 PATCH /groups/{id}/team/channels/{id}，请改用 PATCH /teams/{id}/channels/{id}。 |
|删除|beta|已删除 POST /groups/{id}/team/channels/{id}/chatthreads，请改用 POST /teams/{id}/channels/{id}/chatthreads。 |
|删除|beta|已删除 GET /groups/{id}/team/channels，请改用 GET /teams/{id}/channels。 |
|删除|beta|已删除 DELETE /groups/{id}/channels/{id}，请改用 DELETE /teams/{id}/channels/{id}。 |
|删除项|beta|已删除 GET /groups/{id}/channels/{id}，请改用 GET /teams/{id}/channels/{id}。 |
|删除|beta|已删除 PATCH /groups/{id}/channels/{id}，请改用 PATCH /teams/{id}/channels/{id}。 |
|删除|beta|已删除 POST /groups/{id}/channels/{id}/chatthreads，请改用 POST /teams/{id}/channels/{id}/chatthreads。 |
|删除|beta|已删除 GET /groups/{id}/channels，请改用 GET /teams/{id}/channels。 |
|删除|beta|已删除 POST /groups/{id}/team/channels，请改用 POST /teams/{id}/channels。 |
|删除|beta|已删除 GET /groups/{id}/team，请改用 GET /teams/{id}。 |
|删除项|beta|已删除 PATCH /groups/{id}/team，请改用 PATCH /teams/{id}。 |
|添加项|beta|向[列出组织中的所有团队](teams-list-all-teams.md)添加了 API。 |


## <a name="june-2018"></a>2018 年 6 月

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加|v1.0|向 [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) 实体添加了 **connectorServerName** 属性|
|添加项|v1.0|向 [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0) 实体添加了 **firewallEnabled**、**firewallBlockAllIncoming** 和 **firewallEnableStealthMode** 属性|
|添加项|v1.0|向 [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-1.0) 枚举类型添加了 **unknown** 成员|
|添加项|beta|添加了新实体：<br/>[androidDeviceOwnerWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerwificonfiguration?view=graph-rest-beta)<br/>[iosVppAppAssignedDeviceLicense](/graph/api/resources/intune-apps-iosvppappassigneddevicelicense?view=graph-rest-beta)<br/>[iosVppAppAssignedLicense](/graph/api/resources/intune-apps-iosvppappassignedlicense?view=graph-rest-beta)<br/>[iosVppAppAssignedUserLicense](/graph/api/resources/intune-apps-iosvppappassigneduserlicense?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationstate?view=graph-rest-beta)<br/>[userPFXCertificate](/graph/api/resources/intune-raimportcerts-userpfxcertificate?view=graph-rest-beta)<br/>[vppTokenLicenseSummary](/graph/api/resources/intune-onboarding-vpptokenlicensesummary?view=graph-rest-beta)<br/>|
|添加项|beta|添加了新复杂类型：<br/>[iosVppAppRevokeLicensesActionResult](/graph/api/resources/intune-apps-iosvppapprevokelicensesactionresult?view=graph-rest-beta)<br/>|
|添加项|beta|添加了新枚举类型：<br/>[androidDeviceOwnerSystemUpdateInstallType](/graph/api/resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype?view=graph-rest-beta)<br/>[androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta)<br/>[userPfxIntendedPurpose](/graph/api/resources/intune-raimportcerts-userpfxintendedpurpose?view=graph-rest-beta)<br/>[userPfxPaddingScheme](/graph/api/resources/intune-raimportcerts-userpfxpaddingscheme?view=graph-rest-beta)<br/>|
|添加项|beta|在 [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) 上添加了 [createGooglePlayWebToken](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken?view=graph-rest-beta) 操作 |
|添加项|beta|在 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 上添加了 [revokeAllLicenses](/graph/api/intune-apps-iosvppapp-revokealllicenses?view=graph-rest-beta) 操作 |
|添加项|beta|在 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 上添加了 [revokeUserLicense](/graph/api/intune-apps-iosvppapp-revokeuserlicense?view=graph-rest-beta) 操作 |
|添加项|beta|在 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 上添加了 [revokeDeviceLicense](/graph/api/intune-apps-iosvppapp-revokedevicelicense?view=graph-rest-beta) 操作 |
|添加项|beta|在 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 上添加了 [sendCustomNotificationToCompanyPortal](/graph/api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal?view=graph-rest-beta) 操作 |
|添加项|beta|在 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) 集合上添加了 **getLicensesForApp** 函数 |
|删除|beta|删除了以下枚举类型：<br/>**windowsUpdateInsiderBuildControl**<br/>|
|添加项|beta|向 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **systemUpdateWindowStartMinutesAfterMidnight**、**systemUpdateWindowEndMinutesAfterMidnight** 和 **systemUpdateInstallType** 属性|
|更改项|beta|更改了 [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) 实体上以下属性的类型：<br/>**passwordMinutesOfInactivityBeforeScreenTimeout** 从 Int64 更改为 Int32<br/>|
|添加项|beta|向 [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta) 实体添加了 **customKeyValueData** 属性|
|添加项|beta|向 [androidVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidvpnconfiguration?view=graph-rest-beta) 实体添加了 **customKeyValueData** 属性|
|添加项|beta|向 [androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta) 实体添加了 **customKeyValueData** 属性|
|添加项|beta|向 [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) 实体添加了 **customKeyValueData** 属性|
|添加项|beta|向 [deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta) 实体添加了 **userId** 和 **userPrincipalName** 属性|
|添加项|beta|向 [deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta) 实体添加了 **userId** 和 **userPrincipalName** 属性|
|添加项|beta|向 [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) 实体添加了 **connectorServerName** 属性|
|删除|beta|从 [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) 实体中删除了 **settingXml** 属性|
|添加项|beta|向 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 实体添加了 **vppTokenId** 和 **revokeLicenseActionResults** 属性|
|添加项|beta|向 [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) 实体添加了 **firewallEnabled**、**firewallBlockAllIncoming** 和 **firewallEnableStealthMode** 属性|
|删除|beta|从 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体中删除了 **remoteAssistanceSessionErrorString** 属性|
|添加项|beta|向 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 实体添加了 **antivirusRequired** 和 **antiSpywareRequired** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **defenderOfficeAppsOtherProcessInjection**、**defenderOfficeAppsExecutableContentCreationOrLaunch**、**defenderOfficeAppsLaunchChildProcess**、**defenderOfficeMacroCodeAllowWin32Imports**、**defenderScriptObfuscatedMacroCode**、**defenderScriptDownloadedPayloadExecution**、**defenderProcessCreation**、**defenderUntrustedUSBProcess**、**defenderUntrustedExecutable** 和 **defenderEmailContentExecution** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **searchDisableLocation**、**inkWorkspaceAccessState**、**defenderPotentiallyUnwantedAppActionSetting** 和 **defenderCloudExtendedTimeoutInSeconds** 属性|
|添加项|beta|向 [windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-beta) 实体添加了 **updatesMinimumAutoInstallClassification** 属性|
|删除项|beta|从 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体中删除了 **previewBuildSetting** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **userPfxCertificates** 导航属性|
|添加项|beta|向 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 实体添加了 **assignedLicenses** 导航属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **managedDeviceMobileAppConfigurationStates** 导航属性|
|添加项|beta|向 [iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta) 复杂类型添加了 **websiteList** 属性|
|添加项|beta|向 [devicePlatformType](/graph/api/resources/intune-deviceconfig-deviceplatformtype?view=graph-rest-beta) 枚举类型添加了 **androidWorkProfile** 成员|
|添加项|beta|向 [editionUpgradeLicenseType](/graph/api/resources/intune-deviceconfig-editionupgradelicensetype?view=graph-rest-beta) 枚举类型添加了 **notConfigured** 成员|
|添加项|beta|向 [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-beta) 枚举类型添加了 **unknown** 成员|
|添加项|beta|向 [mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta) 枚举类型添加了 **userRequestedInstall** 成员|
|添加项|beta|向 [windows10EditionType](/graph/api/resources/intune-deviceconfig-windows10editiontype?view=graph-rest-beta) 枚举类型添加了 **notConfigured** 成员

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 向 [Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-beta) 添加了[访问评审](/graph/api/resources/accessreviews-root?view=graph-rest-beta)功能。 |

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项 | 全部 | 新的应用程序权限 _Application.ReadWrite.All_ 和 _Application.ReadWrite.OwnedBy_，允许客户端应用创建、读取、更新和删除应用程序和服务主体，如[权限主题](permissions-reference.md#application-resource-permissions)中所述。 |
| 新增 | v1.0 | 向 [user](/graph/api/resources/user?view=graph-rest-1.0) 资源添加了 **ageGroup**、**legalAgeGroupClassification** 和 **ConsentRequiredForMinor** 属性

### <a name="identity-and-access--privileged-identity-management"></a>身份和访问|特权身份管理

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition | beta | 添加了 [privilegedAccess](/graph/api/resources/privilegedaccess?view=graph-rest-beta) 实体。|
| Addition | beta | 添加了 [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) 实体及以下方法和操作： <br> [List](/graph/api/governanceresource-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceresource-get?view=graph-rest-beta)<br>|
| Addition | beta | 添加了 [governanceSubject](/graph/api/resources/governancesubject?view=graph-rest-beta) 实体。|
| Addition | beta | 添加了 [governanceRoleDefinition](/graph/api/resources/governanceroledefinition?view=graph-rest-beta) 实体及以下方法和操作：<br> [List](/graph/api/governanceroledefinition-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroledefinition-get?view=graph-rest-beta) |
| Addition | beta | 添加了 [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta) 实体及以下方法和操作：<br> [List](/graph/api/governanceroleassignment-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroleassignment-get?view=graph-rest-beta) <br> [Export](/graph/api/governanceroleassignment-export?view=graph-rest-beta) |
| 添加项 | beta | 添加了 [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) 实体及以下方法和操作：<br> [列出](/graph/api/governanceroleassignmentrequest-list?view=graph-rest-beta) <br> [获取](/graph/api/governanceroleassignmentrequest-get?view=graph-rest-beta) <br> [Create](/graph/api/governanceroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/governanceroleassignmentrequest-cancel?view=graph-rest-beta) <br> [更新](/graph/api/governanceroleassignmentrequest-update?view=graph-rest-beta) |
| 添加项 | beta | 添加了 [governanceRoleSetting](/graph/api/resources/governancerolesetting?view=graph-rest-beta) 实体及以下方法和操作：<br> [List](/graph/api/governancerolesetting-list?view=graph-rest-beta) <br> [Get](/graph/api/governancerolesetting-get?view=graph-rest-beta) <br> [更新](/graph/api/governancerolesetting-update?view=graph-rest-beta) |
| 添加项 | beta | 添加了以下复杂类型： <br> [governancePermission](/graph/api/resources/governancepermission?view=graph-rest-beta) <br> [governanceRoleAssignmentRequestStatus](/graph/api/resources/governanceroleassignmentrequeststatus?view=graph-rest-beta) <br> [governanceRuleSetting](/graph/api/resources/governancerulesetting?view=graph-rest-beta) <br> [governanceSchedule](/graph/api/resources/governanceschedule?view=graph-rest-beta)|

### <a name="security"></a>安全性

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Addition        | beta        | 添加了新枚举类型：<br/>[alertFeedback](/graph/api/resources/alertfeedbackenumtype?view=graph-rest-beta)<br/>[alertStatus](/graph/api/resources/alertstatusenumtype?view=graph-rest-beta)<br/>[alertType](/graph/api/resources/alerttypeenumtype?view=graph-rest-beta)<br/>[applicationPermissionsRequired](/graph/api/resources/applicationpermissionsrequiredenumtype?view=graph-rest-beta)<br/>[logonType](/graph/api/resources/logontypeenumtype?view=graph-rest-beta)<br/>[processIntegrityLevel](/graph/api/resources/processintegritylevelenumtype?view=graph-rest-beta)<br/>[securityNetworkProtocol](/graph/api/resources/securitynetworkprotocolenumtype?view=graph-rest-beta)<br/>[userAccountSecurityType](/graph/api/resources/useraccountsecuritytypeenumtype?view=graph-rest-beta)<br/>


### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)
| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|添加         | Beta          | 添加了团队 [archive](/graph/api/team-archive?view=graph-rest-beta) 和 [unarchive](/graph/api/team-unarchive?view=graph-rest-beta) API。|
|添加         | Beta          | 添加了团队 [clone](/graph/api/team-clone?view=graph-rest-beta) 操作。 |
|添加         | Beta          | 添加了 API 以向团队添加或删除 [apps](/graph/api/resources/teamsapp?view=graph-rest-beta)。 |
|更改|Beta|更新了 [team](/graph/api/resources/team?view=graph-rest-beta) 实体的路径。|
|更改项|Beta|更新了[频道](/graph/api/resources/channel?view=graph-rest-beta)实体的路径。|


## <a name="may-2018"></a>2018 年 5 月

### <a name="customer-booking-microsoft-bookings"></a>客户预订（Microsoft Bookings）

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | Beta          | 添加了 [bookingBusiness](/graph/api/resources/bookingbusiness?view=graph-rest-beta) 实体及以下 CRUD 方法和操作： <br> [List](/graph/api/bookingbusiness-list?view=graph-rest-beta) <br> [创建](/graph/api/bookingbusiness-post-bookingbusinesses?view=graph-rest-beta) <br> [获取](/graph/api/bookingbusiness-get?view=graph-rest-beta) <br> [更新](/graph/api/bookingbusiness-update?view=graph-rest-beta) <br> [删除](/graph/api/bookingbusiness-delete?view=graph-rest-beta) <br> [发布](/graph/api/bookingbusiness-publish?view=graph-rest-beta) <br> [取消发布](/graph/api/bookingbusiness-unpublish?view=graph-rest-beta)。 <br> 详细了解关于与 [Microsoft Bookings API](booking-concept-overview.md) 集成的信息。 |
| 添加项        | Beta          | 添加了 [bookingAppointment](/graph/api/resources/bookingappointment?view=graph-rest-beta) 实体及以下 CRUD 方法和操作： <br> [List](/graph/api/bookingbusiness-list-appointments?view=graph-rest-beta) <br> [创建](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta) <br> [获取](/graph/api/bookingappointment-get?view=graph-rest-beta) <br> [更新](/graph/api/bookingappointment-update?view=graph-rest-beta) <br> [删除](/graph/api/bookingappointment-delete?view=graph-rest-beta) <br> [取消](/graph/api/bookingappointment-cancel?view=graph-rest-beta)。 |
| 添加项        | Beta          | 添加了 [bookingCurrency](/graph/api/resources/bookingcurrency?view=graph-rest-beta) 实体和以下方法： <br> [列出](/graph/api/bookingcurrency-list?view=graph-rest-beta) <br> [获取](/graph/api/bookingcurrency-get?view=graph-rest-beta)。 |
| 添加项        | Beta          | 添加了 [bookingCustomer](/graph/api/resources/bookingcustomer?view=graph-rest-beta) 实体和以下 CRUD 方法： <br> [List](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta) <br> [创建](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta) <br> [获取](/graph/api/bookingcustomer-get?view=graph-rest-beta) <br> [更新](/graph/api/bookingcustomer-update?view=graph-rest-beta) <br> [删除](/graph/api/bookingcustomer-delete?view=graph-rest-beta)。|
| 添加项        | Beta          | 添加了 [bookingService](/graph/api/resources/bookingservice?view=graph-rest-beta) 实体和以下 CRUD 方法： <br> [List](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) <br> [创建](/graph/api/bookingbusiness-post-services?view=graph-rest-beta) <br> [获取](/graph/api/bookingservice-get?view=graph-rest-beta) <br> [更新](/graph/api/bookingservice-update?view=graph-rest-beta) <br> [删除](/graph/api/bookingservice-delete?view=graph-rest-beta)。|
| 添加项        | Beta          | 添加了 [bookingStaffMember](/graph/api/resources/bookingstaffmember?view=graph-rest-beta) 实体和以下 CRUD 方法： <br> [List](/graph/api/bookingbusiness-list-staffmembers?view=graph-rest-beta) <br> [创建](/graph/api/bookingbusiness-post-staffmembers?view=graph-rest-beta) <br> [获取](/graph/api/bookingstaffmember-get?view=graph-rest-beta) <br> [更新](/graph/api/bookingstaffmember-update?view=graph-rest-beta) <br> [删除](/graph/api/bookingstaffmember-delete?view=graph-rest-beta)。|
| 添加项        | Beta          | 添加了以下复杂类型： <br> [bookingNamedEntity](/graph/api/resources/bookingnamedentity?view=graph-rest-beta) <br> [bookingPerson](/graph/api/resources/bookingperson?view=graph-rest-beta) <br> [bookingReminder](/graph/api/resources/bookingreminder?view=graph-rest-beta) <br> [bookingWorkHours](/graph/api/resources/bookingworkhours?view=graph-rest-beta) <br> [bookingWorkTimeSlot](/graph/api/resources/bookingworktimeslot?view=graph-rest-beta)。|

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|添加项|beta|添加的新实体：<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)<br/>[easEmailProfileConfigurationBase](/graph/api/resources/intune-deviceconfig-easemailprofileconfigurationbase?view=graph-rest-beta)<br/>[mobileAppIntentAndState](/graph/api/resources/intune-troubleshooting-mobileappintentandstate?view=graph-rest-beta)<br/>[mobileAppTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingevent?view=graph-rest-beta)<br/>[unsupportedDeviceConfiguration](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfiguration?view=graph-rest-beta)<br/>[windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta)<br/>|
|添加项|beta|添加了新复杂类型：<br/>[managedDeviceCleanupSettings](/graph/api/resources/intune-devices-manageddevicecleanupsettings?view=graph-rest-beta)<br/>[mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppPolicyCreationHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapppolicycreationhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppStateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappstatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppTargetHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapptargethistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppUpdateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappupdatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingDeviceCheckinHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingdevicecheckinhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingHistoryItem](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem?view=graph-rest-beta)<br/>[unsupportedDeviceConfigurationDetail](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail?view=graph-rest-beta)<br/>**windowsAutoPilotEnrollmentSettings**<br/>[windowsKioskActiveDirectoryGroup](/graph/api/resources/intune-deviceconfig-windowskioskactivedirectorygroup?view=graph-rest-beta)<br/>[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta)<br/>[windowsKioskAppConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskappconfiguration?view=graph-rest-beta)<br/>[windowsKioskAutologon](/graph/api/resources/intune-deviceconfig-windowskioskautologon?view=graph-rest-beta)<br/>[windowsKioskAzureADGroup](/graph/api/resources/intune-deviceconfig-windowskioskazureadgroup?view=graph-rest-beta)<br/>[windowsKioskAzureADUser](/graph/api/resources/intune-deviceconfig-windowskioskazureaduser?view=graph-rest-beta)<br/>[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)<br/>[windowsKioskLocalGroup](/graph/api/resources/intune-deviceconfig-windowskiosklocalgroup?view=graph-rest-beta)<br/>[windowsKioskLocalUser](/graph/api/resources/intune-deviceconfig-windowskiosklocaluser?view=graph-rest-beta)<br/>[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)<br/>[windowsKioskProfile](/graph/api/resources/intune-deviceconfig-windowskioskprofile?view=graph-rest-beta)<br/>[windowsKioskSingleUWPApp](/graph/api/resources/intune-deviceconfig-windowskiosksingleuwpapp?view=graph-rest-beta)<br/>[windowsKioskUser](/graph/api/resources/intune-deviceconfig-windowskioskuser?view=graph-rest-beta)<br/>[windowsKioskUWPApp](/graph/api/resources/intune-deviceconfig-windowskioskuwpapp?view=graph-rest-beta)<br/>[windowsKioskVisitor](/graph/api/resources/intune-deviceconfig-windowskioskvisitor?view=graph-rest-beta)<br/>|
|添加项|beta 版本|添加了新枚举类型：<br/>[defenderScheduleScanDay](/graph/api/resources/intune-deviceconfig-defenderschedulescanday?view=graph-rest-beta)<br/>[defenderSubmitSamplesConsentType](/graph/api/resources/intune-deviceconfig-defendersubmitsamplesconsenttype?view=graph-rest-beta)<br/>[domainNameSource](/graph/api/resources/intune-deviceconfig-domainnamesource?view=graph-rest-beta)<br/>[localSecurityOptionsSmartCardRemovalBehaviorType](/graph/api/resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype?view=graph-rest-beta)<br/>[mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta)<br/>[mobileAppIntent](/graph/api/resources/intune-troubleshooting-mobileappintent?view=graph-rest-beta)<br/>[roleAssignmentScopeType](/graph/api/resources/intune-rbac-roleassignmentscopetype?view=graph-rest-beta)<br/>[usernameSource](/graph/api/resources/intune-deviceconfig-usernamesource?view=graph-rest-beta)<br/>[windowsDeviceUsageType](/graph/api/resources/intune-enrollment-windowsdeviceusagetype?view=graph-rest-beta)<br/>|
|添加项|beta|添加了 [setDeviceName](/graph/api/intune-devices-manageddevice-setdevicename?view=graph-rest-beta)<br/>操作到 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|删除|beta|删除了以下实体：<br/>**depEnrollmentProfile**<br/>**enrollmentProfile**<br/>**importedAppleDeviceIdentity**<br/>**importedAppleDeviceIdentityResult**<br/>|
|删除|beta|删除了以下复杂类型：<br/>**managementCertificateWithThumbprint**<br/>|
|删除|beta|删除了以下枚举类型：<br/>**depTokenType**<br/>**discoverySource**<br/>**iTunesPairingMode**<br/>|
|删除|beta|在 [importedAppleDeviceIdentity](/graph/api/resources/intune-corpenrollment-importedappledeviceidentity?view=graph-rest-beta) 集合上删除了 importAppleDeviceIdentityList 操作 |
|删除|beta|在 [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) 上删除了 [updateDeviceProfileAssignment](/graph/api/intune-corpenrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) 操作 |
|删除|beta|在 [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) 上删除了 setDefaultProfile 操作 |
|删除|beta|在 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 上删除了 shareForSchoolDataSyncService 操作 |
|删除|beta|在 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 上删除了 unshareForSchoolDataSyncService 操作 |
|删除|beta|在 [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) 上删除了 exportMobileConfig](/graph/api/intune_corpenrollment_enrollmentprofile_exportmobileconfig?view=graph-rest-beta) 函数 |
|添加项|beta|向 [androidEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-androideasemailprofileconfiguration?view=graph-rest-beta) 实体添加了 **userDomainNameSource** 和 **customDomainName** 属性|
|Addition|beta|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBlockCamera** 和 **workProfileBlockCrossProfileContactsSearch** 属性|
|添加项|beta|向 [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBlockCamera** 和 **workProfileBlockCrossProfileContactsSearch** 属性|
|添加项|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **thirdPartyKeyboardsBlocked** 和 **filterOpenInToOnlyManagedApps** 属性|
|添加项|beta|向 [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) 实体添加了 **conflictCount** 属性|
|添加项|beta|向 [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) 实体添加了 **conflictCount** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **managedDeviceCleanupSettings** 属性|
|删除|beta|从 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体中删除了 **usernameSource** 属性|
|添加项|beta|向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **thirdPartyKeyboardsBlocked** 和 **filterOpenInToOnlyManagedApps** 属性|
|添加项|beta|向 [macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta) 实体添加了 **ignoreVersionDetection** 属性|
|添加项|beta|向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体添加了 **pinRequiredOnLaunchInsteadOfBiometric** 和 **pinRequiredInsteadOfBiometricTimeout** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **autopilotEnrolled**、**requireUserEnrollmentApproval**、**iccid** 和 **udid** 属性|
|删除|beta|从 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体中删除了 **isAutopilotEnrolled** 属性|
|添加项|beta|向 [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta) 实体添加了 **notApplicablePlatformCount** 和 **conflictCount** 属性|
|添加项|beta|向 [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta) 实体添加了 **conflictCount** 属性|
|添加项|beta|向 [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) 实体添加了 **scopeType** 属性|
|删除|beta|从 [windows10EasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windows10easemailprofileconfiguration?view=graph-rest-beta) 实体中删除了 **usernameSource** 属性|
|加|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees**、**localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers**、**localSecurityOptionsDisableServerDigitallySignCommunicationsAlways**、**localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees**、**localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares**、**localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts**、**localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares**、**localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange** 和 **localSecurityOptionsSmartCardRemovalBehavior** 属性|
|加|beta|向 [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) 实体添加了 **showInstallationProgress**、**blockDeviceSetupRetryByUser**、**allowDeviceResetOnInstallFailure**、**allowLogCollectionOnInstallFailure**、**customErrorMessage**、**installProgressTimeoutInMinutes** 和 **allowDeviceUseOnInstallFailure** 属性|
|删除|beta|从 [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) 实体中删除了 **title**、**bodyText**、**moreInfoUrl** 和 **moreInfoText** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **defenderBlockOnAccessProtection**、**defenderScheduleScanDay** 和 **defenderSubmitSamplesConsentType** 属性|
|加|beta|向 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 添加了 **language** 和 **enrollmentSettings** 属性|
|加|beta|向 [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) 实体添加了 **useDeviceContext** 属性|
|删除|beta|从 [windowsPhoneEASEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration?view=graph-rest-beta) 实体中删除了 **usernameSource** 属性|
|删除|beta|从 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体中删除了 **localActions** 导航属性|
|删除|beta|从 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体中删除了 **enrollmentProfiles** 和 **importedAppleDeviceIdentities** 导航属性|
|加|beta|向 [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) 实体添加了 **mobileAppIntentAndStates** 和 **mobileAppTroubleshootingEvents** 导航属性|
|加|beta|向 [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 复杂类型添加了 **deviceUsageType** 和 **skipKeyboardSelectionPage** 属性|
|删除|beta|从 [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta) 枚举类型中删除了 **paloAltoGlobalProtect** 成员|
|加|beta|向 [androidUsernameSource](/graph/api/resources/intune-deviceconfig-androidusernamesource?view=graph-rest-beta) 枚举类型添加了 **samAccountName** 和 **primarySmtpAddress** 成员|
|删除|beta|从 [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta) 枚举类型中删除了 **paloAltoGlobalProtect** 成员|
|添加项|beta|向 [windows10VpnConnectionType](/graph/api/resources/intune-deviceconfig-windows10vpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **paloAltoGlobalProtect** 成员|

### <a name="education"></a>教育

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改          | v1.0 和 beta | 必须有 **Members.Read.Hidden** 范围，才能使用仅应用令牌对 [educationClass](/graph/api/resources/educationclass?view=graph-rest-1.0) 实体读取或更新 **Members** 集合。 |
|Change           |Beta           |更新了 [educationsubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) 状态属性中 **educationSubmissionStatus** 类型的可能值。|
|Change           |Beta 版本           |向 [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta) 的 assignTo 属性添加了 **educationAssignmentIndividualRecipient** 复杂类型。|
|Change           |Beta 版本           |添加了 [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) 的 **unsubmittedBy**、**unsubmittedDate**、**returnedBy**、**returnedDate** 属性。|
|添加项         |Beta           |向 [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) 添加了 [return](/graph/api/educationsubmission-return?view=graph-rest-beta) 和 [unsubmit](/graph/api/educationsubmission-unsubmit?view=graph-rest-beta) 操作。|
|更改           |Beta 版本           |删除了 [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) 上的 release 和 recall 操作。|

### <a name="groups"></a>组

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | 向[发布](/graph/api/resources/post?view=graph-rest-1.0)实体添加****“重要性”属性。 |

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Change           | beta          | 已将 [subscription](/graph/api/resources/subscription?view=graph-rest-beta) 实体的 **creatorUserId** 属性重命名为 **creatorId**，以更好地反映含义。 |

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0        | 向[目录（已删除项目）](/graph/api/resources/directory?view=graph-rest-1.0)资源添加了[列出用户所拥有的已删除项](/graph/api/directory-deleteditems-user-owned?view=graph-rest-1.0)操作 |
| 加 | beta | 向 [directory](/graph/api/resources/directory?view=graph-rest-beta) 资源添加了 [getUserOwnedObjects](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) 函数，以列出给定用户拥有的已删除组。 |

### <a name="social-and-workplace-intelligence--insights"></a>社交和工作场所智能|见解

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | Beta          | 添加了 [settings](/graph/api/resources/user-settings?view=graph-rest-beta) 实体和以下 CRUD 方法： <br> [获取](/graph/api/user-get-settings?view=graph-rest-beta) <br> [更新](/graph/api/user-update-settings?view=graph-rest-beta) |


## <a name="april-2018"></a>2018 年 4 月

### <a name="calendar-outlook"></a>日历 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0          | 向 [event](/graph/api/resources/event?view=graph-rest-1.0) 实体添加了 **locations** 属性，以支持组织与会者可以从多个位置参加的事件。 |
| 添加        | v1.0          | 向 [location](/graph/api/resources/location?view=graph-rest-1.0) 复杂类型添加了 **locationType** 属性。 |
| 添加        | v1.0          | 向 [location](/graph/api/resources/location?view=graph-rest-1.0) 复杂类型添加了 **uniqueId** 和 **uniqueIdType** 属性。 在这种情况下，这些属性仅供内部使用。 |

### <a name="cross-device-experiences-project-rome"></a>跨设备体验 (Project Rome)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加 | v1.0 | 添加了[获取最近的活动 API](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0) |
| 添加 | v1.0 | 添加了[获取活动 API](/graph/api/projectrome-get-activities?view=graph-rest-1.0) |
| 添加 | v1.0 | 添加了 [Upsert 活动](/graph/api/projectrome-put-activity?view=graph-rest-1.0) |
| 添加 | v1.0 | 添加了 [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-1.0) |
| 添加 | v1.0 | 添加了[删除活动](/graph/api/projectrome-delete-activity?view=graph-rest-1.0) |
| 添加 | v1.0 | 添加了 [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-1.0) |
| 添加 | v1.0 | 添加了[活动](/graph/api/resources/projectrome-activity?view=graph-rest-1.0) |
| 添加项 | v.10 | 添加了 [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-1.0) |
| 添加 | v1.0 | 添加了 [visualInfo](/graph/api/resources/projectrome-visualinfo?view=graph-rest-1.0) |
| 添加项 | v1.0 | 添加了 [imageInfo](/graph/api/resources/projectrome-imageinfo?view=graph-rest-1.0) |
| 添加项 | v.10 | 添加了 [Project Rome 概述](/graph/api/resources/project-rome-overview?view=graph-rest-1.0) |
| 更改 | Beta | 向 [Upsert 活动](/graph/api/projectrome-put-activity?view=graph-rest-beta)添加了深层插入文档 |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|添加|v1.0|添加的新实体：<br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-1.0)<br/>|
|添加|v1.0|添加的新枚举类型：<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-1.0)<br/>|
|添加|v1.0|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 实体添加了 **managedDeviceOwnerType** 属性|
|添加|v1.0|将 **deviceStatuses** 导航属性添加到 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0) 实体|
|添加|v1.0|向 [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-1.0) 枚举类型添加了 **androidWorkProfile** 成员|
|Addition|beta|添加的新实体：<br/>[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofileeasemailprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate?view=graph-rest-beta)<br/>[androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilewificonfiguration?view=graph-rest-beta)<br/>[restrictedAppsViolation](/graph/api/resources/intune-deviceconfig-restrictedappsviolation?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta)<br/>|
|Addition|beta|新增了复杂类型：<br/>[managedDeviceModelsAndManufacturers](/graph/api/resources/intune-devices-manageddevicemodelsandmanufacturers?view=graph-rest-beta)<br/>[managedDeviceReportedApp](/graph/api/resources/intune-devices-manageddevicereportedapp?view=graph-rest-beta)<br/>[windowsEnrollmentStatusScreenSettings](/graph/api/resources/intune-enrollment-windowsenrollmentstatusscreensettings?view=graph-rest-beta)<br/>|
|Addition|beta|添加的新枚举类型：<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-beta)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-beta)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-beta)<br/>[androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)<br/>[bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>[localSecurityOptionsInformationShownOnLockScreenType](/graph/api/resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype?view=graph-rest-beta)<br/>[managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-beta)<br/>[restrictedAppsState](/graph/api/resources/intune-deviceconfig-restrictedappsstate?view=graph-rest-beta)<br/>[windows10VpnProfileTarget](/graph/api/resources/intune-deviceconfig-windows10vpnprofiletarget?view=graph-rest-beta)<br/>|
|添加项|beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [playLostModeSound](/graph/api/intune-devices-manageddevice-playlostmodesound?view=graph-rest-beta) 操作 |
|删除|beta|删除了以下枚举类型：<br/>**bitLockerRecoveryinformationType**<br/>**windowsUpdateRestartMode**<br/>|
|添加项|beta|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBlockScreenCapture** 和 **workProfileBlockCrossProfileCallerId** 属性|
|添加项|beta|向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **minimumWipePatchVersion**、**allowedAndroidDeviceManufacturers** 和 **appActionIfAndroidDeviceManufacturerNotAllowed** 属性|
|添加项|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **minimumWipeSdkVersion**、**minimumWipePatchVersion**、**allowedIosDeviceModels**、**appActionIfIosDeviceModelNotAllowed**、**allowedAndroidDeviceManufacturers** 和 **appActionIfAndroidDeviceManufacturerNotAllowed** 属性|
|添加项|beta|向 [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) 实体添加了 **notApplicablePlatformCount** 和 **conflictCount** 属性|
|添加项|beta|向 [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) 实体添加了 **notApplicablePlatformCount** 和 **conflictCount** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **accountMoveCompletionDateTime** 属性|
|添加项|beta|向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **minimumWipeSdkVersion**、**allowedIosDeviceModels** 和 **appActionIfIosDeviceModelNotAllowed** 属性|
|添加项|beta|向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体添加了 **minimumWipeOsVersion**、**minimumWipeAppVersion**、**appActionIfDeviceComplianceRequired** 和 **appActionIfMaximumPinRetriesExceeded** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **managedDeviceOwnerType**、**preferMdmOverGroupPolicyAppliedDateTime**、**isAutopilotEnrolled** 和 **requestUserEnrollmentApproval** 属性|
|添加项|beta|向 [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) 实体添加了 **managedDeviceModelsAndManufacturers** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **localSecurityOptionsMachineInactivityLimitInMinutes**、**localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool**、**localSecurityOptionsInformationShownOnLockScreen**、**defenderSecurityCenterDisableAccountUI**、**defenderSecurityCenterDisableHardwareUI**、**defenderSecurityCenterDisableRansomwareUI**、**defenderSecurityCenterDisableSecureBootUI** 和 **defenderSecurityCenterDisableTroubleshootingUI** 属性|
|添加项|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **printerNames**、**printerDefaultName**、**printerBlockAddition** 和 **searchBlockWebResults** 属性|
|添加项|beta|向 [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) 实体添加了 **profileTarget**、**enableAlwaysOn** 和 **enableDeviceTunnel** 属性|
|添加项|beta|向 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 实体添加了 **enrollmentStatusScreenSettings** 属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceConfigurationRestrictedAppsViolations** 导航属性|
|添加项|beta|向 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 实体添加了 **assignments** 导航属性|
|添加项|beta|向 [windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta) 实体添加了 **networkAccessConfigurations** 导航属性|
|删除|beta|从 [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta) 复杂类型删除**权限**属性|
|更改|beta 版本|更改了 [bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta) 复杂类型上以下属性的类型：<br/>**recoveryInformationToStore** 从 [bitLockerRecoveryinformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta) 更改为 [bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>|
|添加项|beta|向 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型添加了 **deviceInactivityBeforeRetirementInDay** 属性|
|添加项|beta|向 [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) 复杂类型添加了 **landingPageCustomizedImage** 属性|
|删除|beta|从 [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta) 复杂类型删除了 **ipAddressOrFqdn** 属性|
|删除|beta|从 [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) 复杂类型删除了 **restartMode** 属性|
|添加项|beta|向 [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **paloAltoGlobalProtect** 成员|
|添加项|beta|向 [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **paloAltoGlobalProtect** 成员|
|添加项|beta|向 [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) 枚举类型添加了 **paloAltoGlobalProtect** 成员|
|添加项|beta|向 [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-beta) 枚举类型添加了 **androidWorkProfile** 成员|

### <a name="education"></a>教育

|更改类型|版本|说明|
|:---|:---|:---|
|更改|Beta|向 [educationsynchronizationerror](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta) 添加了 reportableIdentifier 属性。|
|更改|Beta|更新了 [uploadUrl](/graph/api/educationsynchronizationprofile-uploadurl?view=graph-rest-beta) API 的响应选项。|
|更改|Beta|更新了 [educationSynchronizationError](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta) 资源类型的说明文本。|
|更改|Beta|更新了[获取同步错误](/graph/api/educationsynchronizationerrors-get?view=graph-rest-beta) API 的说明文本。|

### <a name="identity-and-access--audit-logs"></a>标识和访问|审核日志

|更改类型|版本|Description|
|:---|:---|:---|
|添加|Beta|添加了 [directoryAudit](/graph/api/resources/directoryaudit?view=graph-rest-beta) 和 [signIn](/graph/api/resources/signin?view=graph-rest-beta) 实体以支持新审核日志 API。 |
|添加|Beta|添加以下资源以支持审核日志 API：[appIndentity](/graph/api/resources/appidentity?view=graph-rest-beta)、[auditActivityInitiator](/graph/api/resources/auditactivityinitiator?view=graph-rest-beta)、[conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)、[deviceDetail](/graph/api/resources/devicedetail?view=graph-rest-beta)、[mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta)、[modifiedProperty](/graph/api/resources/modifiedproperty?view=graph-rest-beta)、[signinLocation](/graph/api/resources/signinlocation?view=graph-rest-beta)、[signinStatus](/graph/api/resources/signinstatus?view=graph-rest-beta)、[targetResource](/graph/api/resources/targetresource?view=graph-rest-beta)、[targetResourceApp](/graph/api/resources/targetresourceapp?view=graph-rest-beta)、[targetResourceDevice](/graph/api/resources/targetresourcedevice?view=graph-rest-beta)、[targetResourceDirectory](/graph/api/resources/targetresourcedirectory?view=graph-rest-beta)、[targetResourceGroup](/graph/api/resources/targetresourcegroup?view=graph-rest-beta)、[targetResourceOther](/graph/api/resources/targetresourceother?view=graph-rest-beta)、[targetResourcePolicy](/graph/api/resources/targetresourcepolicy?view=graph-rest-beta)、[targetResourceRole](/graph/api/resources/targetresourcerole?view=graph-rest-beta)、[targetResourceServicePrincipal](/graph/api/resources/targetresourceserviceprincipal?view=graph-rest-beta)、[targetResourceUser](/graph/api/resources/targetresourceuser?view=graph-rest-beta)、[userIdentity](/graph/api/resources/useridentity?view=graph-rest-beta) |

### <a name="identity-and-access-directory-apis"></a>身份和访问 (目录 API)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 向 [organization](/graph/api/resources/organization?view=graph-rest-1.0) 实体添加了 **privacyProfile** 复杂类型。 |
| 添加项        | v1.0        | 向 [user](/graph/api/resources/user?view=graph-rest-1.0) 实体添加了 **legalAgeGroup、ageGroup 和 consentProvidedForMinor** 复杂类型。 |
| 添加项        | v1.0        | 向 [webhook](/graph/api/resources/webhooks?view=graph-rest-1.0) 通知订阅添加了用户和组支持。 |
| 添加项        | beta        | 向[目录（已删除项目）](/graph/api/resources/directory?view=graph-rest-beta)资源添加了[列出用户所拥有的已删除项](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta)操作 |

### <a name="mail-outlook"></a>邮件 (Outlook)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0          | 向 [message](/graph/api/resources/message?view=graph-rest-1.0) 实体添加了 **flag** 属性。 添加了共享的 [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) 复杂类型。|
| 添加项        | v1.0        | 向 [message](/graph/api/resources/message?view=graph-rest-1.0) 实体添加了 **internetMessageHeaders** 属性。 |
| 添加项        | v1.0        | 添加了 [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-1.0) 复杂类型。 |
| 添加项        | v1.0        | 向 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) 实体添加了 **messageRules** 导航属性。 **messageRules** 是 [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) 实例的集合。 |
| 添加项        | v1.0        | 添加了 [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) 实体，以及 [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-1.0)、[messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0) 和 [sizeRange](/graph/api/resources/sizerange?view=graph-rest-1.0) 复杂类型。 |
| 添加项        | v1.0        | 添加了消息规则的以下 CRUD 操作：[创建](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0)、[列出](/graph/api/mailfolder-list-messagerules?view=graph-rest-1.0)、[获取](/graph/api/messagerule-get?view=graph-rest-1.0)、[更新](/graph/api/messagerule-update?view=graph-rest-1.0)和[删除](/graph/api/messagerule-delete?view=graph-rest-1.0)。 |
| 添加 | Beta | 添加了 [mailSearchFolder](/graph/api/resources/mailsearchfolder?view=graph-rest-beta)。 |
| 添加 | Beta | 为邮件搜索文件夹添加了以下 API：[创建](/graph/api/mailsearchfolder-post?view=graph-rest-beta)、[更新](/graph/api/mailsearchfolder-update?view=graph-rest-beta)。 |
| 更改 | Beta | 为邮件搜索文件夹添加了以下支持：[删除邮件文件夹](/graph/api/mailfolder-delete?view=graph-rest-beta)、[获取邮件文件夹](/graph/api/mailfolder-get?view=graph-rest-beta)和[列出子文件夹](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta)。 |

### <a name="personal-contacts-outlook"></a>个人联系人 (Outlook)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0          | 向 [contact](/graph/api/resources/contact?view=graph-rest-1.0) 实体添加了 **flag** 属性。 添加了共享的 [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) 复杂类型。|

### <a name="reports"></a>报告
|更改类型|版本|Description|
|:---|:---|:---|
|添加项|beta| 添加了委派的访问支持。 |
|添加项|v1.0| 添加了委派的访问支持。 |

### <a name="security"></a>安全性

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta       | 添加了[安全 API](/graph/api/resources/security-api-overview?view=graph-rest-beta)，包括以下资源和操作：<br/>[警报](/graph/api/resources/alert?view=graph-rest-beta)（和相关实体）<br/>[获取警报](/graph/api/alert-get?view=graph-rest-beta)<br/>[列出警报](/graph/api/alert-list?view=graph-rest-beta)<br/>[更新警报](/graph/api/alert-update?view=graph-rest-beta)<br/><br/>添加了以下支持文档：<br/>[错误](/graph/api/resources/security-error-codes?view=graph-rest-beta)<br/>[使用 Microsoft Graph 安全性 API 实现安全解决方案集成](security-integration.md)

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|添加了新的 [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta) 实体。|
|添加项|Beta|添加了新的 [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-beta) 实体。|
|添加项|Beta|添加了新的 [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-beta) 实体。|
|添加项|Beta|添加了新的 [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-beta) 实体。|
|添加项|Beta|添加了新的[删除频道](/graph/api/channel-delete?view=graph-rest-beta)操作。|
|添加项|Beta|添加了新的[修补频道](/graph/api/channel-patch?view=graph-rest-beta)操作。|
|添加项|Beta|向 [team](/graph/api/resources/team?view=graph-rest-beta) 资源添加了新的 webUrl 属性。|
|更改|Beta|更新了[频道](/graph/api/resources/channel?view=graph-rest-beta)实体的路径。|

### <a name="users--outlook-settings"></a>用户|Outlook 设置

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 向 [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0) 实体添加了新的 **masterCategories** 导航属性。 **masterCategories** 是 [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) 对象的集合。 |
| 添加项        | v1.0        | 添加了 [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) 实体。 |
| 添加项        | v1.0        | 添加了 [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) 的以下 CRUD 操作：[创建](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0)、[获取](/graph/api/outlookcategory-get?view=graph-rest-1.0)、[更新](/graph/api/outlookcategory-update?view=graph-rest-1.0)和[删除](/graph/api/outlookcategory-delete?view=graph-rest-1.0)。 |
| 添加项        | v1.0        | 向 [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0) 实体添加了新的 [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-1.0) 函数。 |
| 添加项        | v1.0        | 向 [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0) 实体添加了新的 [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-1.0) 函数。 |
|添加项 | v1.0 | 向 [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) 添加了新的 **workingHours** 属性。 请参阅 [workingHours 资源类型](/graph/api/resources/workinghours?view=graph-rest-1.0)，获取有关受支持用例的信息。|
|添加项 | v1.0 | 添加了以下新复杂类型： <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-1.0) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-1.0) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-1.0) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-1.0)|


## <a name="march-2018"></a>2018 年 3 月

### <a name="cross-device-experiences-project-rome"></a>跨设备体验 (Project Rome)

| **更改类型** | **Version** | **说明**              |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta       | 添加了[获取最近的活动 API](/graph/api/projectrome-get-recent-activities?view=graph-rest-beta) |
| 添加项        | Beta       | 添加了[获取活动 API](/graph/api/projectrome-get-activities?view=graph-rest-beta) |
| 更改 | Beta | 向 [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) 添加了 UserActivity.ReadWrite.CreatedByApp 权限 |
| 更改 | Beta | 向 [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta) 添加了 UserActivity.ReadWrite.CreatedByApp 权限 |
| 更改 | Beta | 向 [Delete Activity](/graph/api/projectrome-delete-activity?view=graph-rest-beta) 添加了 UserActivity.ReadWrite.CreatedByApp 权限 |
| 更改 | Beta | 向 [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) 添加了 UserActivity.ReadWrite.CreatedByApp 权限 |
| 更改 | Beta | 向 [activity](/graph/api/resources/projectrome-activity?view=graph-rest-beta) 添加了 **status** 属性 |
| 更改 | Beta | 向 [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) 添加了 **activity** 导航属性 |
| 更改项 | Beta | 向 [Project Rome 概述](/graph/api/resources/project-rome-overview?view=graph-rest-beta)添加了新 API |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|v1.0|添加了新实体：<br/>[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-1.0)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0)<br/>|
|添加项|v1.0|新增了复杂类型：<br/>[appConfigurationSettingItem](/graph/api/resources/intune-apps-appconfigurationsettingitem?view=graph-rest-1.0)<br/>|
|添加项|v1.0|在 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0) 上添加了 [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-1.0) 操作 |
|添加项|v1.0|向 [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0) 实体添加了 **vppTokens** 导航属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **managementCertificateExpirationDate** 属性|
|添加项|beta|向 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型添加了 **enhancedJailBreak** 属性|
|添加项|beta|添加的新实体：<br/>[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)<br/>[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta)<br/>[androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta)<br/>[dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta)<br/>[macOSImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-macosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>[managedEBookCategory](/graph/api/resources/intune-books-managedebookcategory?view=graph-rest-beta)<br/>[microsoftStoreForBusinessContainedApp](/graph/api/resources/intune-apps-microsoftstoreforbusinesscontainedapp?view=graph-rest-beta)<br/>[mobileContainedApp](/graph/api/resources/intune-apps-mobilecontainedapp?view=graph-rest-beta)<br/>[windowsUniversalAppXContainedApp](/graph/api/resources/intune-apps-windowsuniversalappxcontainedapp?view=graph-rest-beta)<br/>|
|添加项|beta|添加的新复杂类型：<br/>[androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceAndAppManagementData](/graph/api/resources/intune-onboarding-deviceandappmanagementdata?view=graph-rest-beta)<br/>[loggedOnUser](/graph/api/resources/intune-devices-loggedonuser?view=graph-rest-beta)<br/>[macOSFirewallApplication](/graph/api/resources/intune-deviceconfig-macosfirewallapplication?view=graph-rest-beta)<br/>[macOSLobChildApp](/graph/api/resources/intune-apps-macoslobchildapp?view=graph-rest-beta)<br/>[macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsappxappassignmentsettings?view=graph-rest-beta)<br/>[windowsUniversalAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsuniversalappxappassignmentsettings?view=graph-rest-beta)<br/>|
|添加项|beta|在 [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) 上添加了 [requestSignupUrl](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl?view=graph-rest-beta) 操作 |
|添加项|beta|在 [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) 上添加了 [completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup?view=graph-rest-beta) 操作 |
|添加项|beta|在 [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) 上添加了 [syncApps](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps?view=graph-rest-beta) 操作 |
|添加项|beta|在 [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) 上添加了 [unbind](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind?view=graph-rest-beta) 操作 |
|添加项|beta|在 [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) 上添加了 [revokeToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken?view=graph-rest-beta) 操作 |
|添加项|beta|在 [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) 上添加了 [createToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken?view=graph-rest-beta) 操作 |
|添加项|beta|在 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) 操作 |
|添加项|beta|在 [dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta) 上添加了 [consentToDataSharing](/graph/api/intune-devices-datasharingconsent-consenttodatasharing?view=graph-rest-beta) 操作 |
|添加项|beta|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) 上添加了 [getLoggedOnManagedDevices](/graph/api/intune-devices-user-getloggedonmanageddevices?view=graph-rest-beta) 函数 |
|添加项|beta|在 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 上添加了 [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) 函数 |
|添加项|beta|在 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 上添加了 [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) 函数 |
|删除|beta|删除了以下实体：<br/>**appleVolumePurchaseProgramToken**<br/>**mdmAppConfigGroupAssignment**<br/>**windows10KioskConfiguration**<br/>|
|删除|beta|在 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 上删除了 [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) 操作 |
|删除|beta|在 [appleVolumePurchaseProgramToken](/graph/api/resources/intune-onboarding-applevolumepurchaseprogramtoken?view=graph-rest-beta) 上添加了 [syncApps](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-syncapps?view=graph-rest-beta) 操作 |
|添加项|beta|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBluetoothEnableContactSharing** 属性|
|添加项|beta|向 [androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta) 实体添加了 **intendedPurpose** 属性|
|添加项|beta|向 [androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta) 实体添加了 **intendedPurpose** 属性|
|添加项|beta|向 [iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta) 实体添加了 **intendedPurpose** 属性|
|添加项|beta|向 [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) 实体添加了 **encodedSettingXml** 属性|
|添加项|beta|向 [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) 实体添加了 **managedDeviceId** 和 **azureADDeviceId** 属性|
|添加项|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **usersLoggedOn** 属性|
|删除|beta|从 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体中删除了 **lastLoggedOnUserId** 属性|
|添加项|beta|向 [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) 实体添加了 **lastModifiedDateTime** 属性。|
|添加项|beta|向 [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) 实体添加了 **isDependency** 属性|
|添加项|beta|向 [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta) 实体添加了 **windowsEnabled**、**macEnabled**、**windowsDeviceBlockedOnMissingPartnerData** 和 **macDeviceBlockedOnMissingPartnerData** 属性|
|添加项|beta|向 [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) 实体添加了 **shouldUninstallOlderVersionsOfOffice** 属性|
|添加项|beta|向 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) 实体添加了 **dataSharingConsentGranted** 属性|
|添加项|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **localSecurityOptionsBlockRemoteLogonWithBlankPassword**、**localSecurityOptionsAdministratorAccountName**、**localSecurityOptionsEnableGuestAccount**、**localSecurityOptionsGuestAccountName**、**localSecurityOptionsAllowUndockWithoutHavingToLogon**、**localSecurityOptionsBlockUsersInstallingPrinterDrivers**、**localSecurityOptionsBlockRemoteOpticalDriveAccess**、**localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser**、**localSecurityOptionsMachineInactivityLimit**、**localSecurityOptionsDoNotRequireCtrlAltDel**、**localSecurityOptionsInformationDisplayedOnLockScreen**、**localSecurityOptionsHideLastSignedInUser**、**localSecurityOptionsHideUsernameAtSignIn**、**localSecurityOptionsLogOnMessageTitle**、**localSecurityOptionsLogOnMessageText**、**localSecurityOptionsAllowPKU2UAuthenticationRequests**、**localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager**、**localSecurityOptionsClearVirtualMemoryPageFile**、**localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn**、**localSecurityOptionsAllowUIAccessApplicationElevation**、**localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations**、**localSecurityOptionsOnlyElevateSignedExecutables**、**localSecurityOptionsAdministratorElevationPromptBehavior**、**localSecurityOptionsStandardUserElevationPromptBehavior**、**localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation**、**localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation**、**localSecurityOptionsAllowUIAccessApplicationsForSecureLocations**、**localSecurityOptionsUseAdminApprovalMode**、**localSecurityOptionsUseAdminApprovalModeForAdministrators**、**deviceGuardLocalSystemAuthorityCredentialGuardSettings**、**deviceGuardEnableVirtualizationBasedSecurity** 和 **deviceGuardEnableSecureBootWithDMA** 属性|
|删除|beta|从 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体中删除了 **defenderPasswordProtectedEmailContentExecutionType** 属性|
|添加项|beta|向 [windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta) 实体添加了 **intendedPurpose** 属性|
|删除|beta|从 [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) 实体中删除了 **printerNames**、**defaultPrinterName** 和 **blockAddingNewPrinter** 属性|
|添加项|beta|向 [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) 实体添加了 **certificateStore** 属性|
|添加项|beta|向 [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) 实体添加了 **purchaseOrderIdentifier** 属性|
|更改|beta|更改了 [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta) 实体上的以下属性：<br/>将 **subjectAlternativeNameType** 从必需更改为可选<br/>|
|添加项|beta|向 [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta) 实体添加了 **advancedThreatProtectionOnboardingFilename** 和 **advancedThreatProtectionOffboardingFilename** 属性|
|添加项|beta|向 [windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta) 实体添加了 **intendedPurpose** 属性|
|添加项|beta|向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **skipChecksBeforeRestart** 和 **updateWeeks** 属性|
|添加项|beta|向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **managedEBookCategories** 导航属性|
|添加项|beta|向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **androidManagedStoreAccountEnterpriseSettings**、**androidManagedStoreAppConfigurationSchemas**、**androidDeviceOwnerEnrollmentProfiles**、**dataSharingConsents** 和 **deviceConfigurationUserStateSummaries** 导航属性|
|删除|beta|从 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体中删除了 **deviceSetupConfigurations** 导航属性|
|删除|beta|从 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 实体中删除了 **groupAssignments** 导航属性|
|添加项|beta|向 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) 实体添加了 **categories** 导航属性|
|添加项|beta|向 [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta) 实体添加了 **containedApps** 导航属性|
|添加项|beta|向 [mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-beta) 实体添加了 **containedApps** 导航属性|
|添加项|beta|向 [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) 实体添加了 **committedContainedApps** 导航属性|

### <a name="files-onedrive-for-business"></a>文件 (OneDrive for Business)
|更改类型|版本|说明|
|:---|:---|:---|
|添加|v1.0|添加的新实体：<br/>[baseItemVersion](/graph/api/resources/baseitemversion?view=graph-rest-1.0)<br/>[driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0)<br/>[listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0)<br/> |
|添加项|v1.0|新增了复杂类型：<br/>[publicationFacet](/graph/api/resources/publicationfacet?view=graph-rest-1.0)<br/> |
|添加项|v1.0|向 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 实体添加了 <b>publication</b> 属性 |
|添加项|v1.0|向 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 实体添加了 <b>versions</b> 导航属性 |
|添加项|v1.0|向 [listItem](/graph/api/resources/listitem?view=graph-rest-1.0) 实体添加了 <b>versions</b> 导航属性 |
|添加项|v1.0|向 [siteCollection](/graph/api/resources/sitecollection?view=graph-rest-1.0) 实体添加了 <b>root</b> 属性 |
|添加项|v1.0|向 [driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0) 实体添加了 [restoreVersion](/graph/api/driveitemversion-restore?view=graph-rest-1.0) 操作 |
|添加项|v1.0|向 [listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0) 实体添加了 [restoreVersion](/graph/api/listitemversion-restore?view=graph-rest-1.0) 操作 |
|添加项|beta|新增了复杂类型：<br/>[itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-beta)<br/> |
|添加项|beta|向 [contentTypeInfo](/graph/api/resources/contenttypeinfo?view=graph-rest-beta) 复杂类型添加了 <b>name</b> 属性。 |
|添加项|beta|向 [deleteAction](/graph/api/resources/deleteaction?view=graph-rest-beta) 复杂类型添加了 <b>objectType</b> 属性 |
|添加项|beta|向 [renameAction](/graph/api/resources/renameaction?view=graph-rest-beta) 复杂类型添加了 <b>newName</b> 属性 |
|添加项|beta|向 [sharepointIds](/graph/api/resources/renameaction?view=graph-rest-beta) 复杂类型添加了 <b>tenantId</b> 属性 |
|添加项|beta|向 [itemActivityTimeSet](/graph/api/resources/itemactivitytimeset?view=graph-rest-beta) 复杂类型添加了 <b>lastRecordedDateTime</b> 属性 |
|添加项|beta|向 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 实体添加了 [preview](/graph/api/driveitem-preview?view=graph-rest-beta) 操作 |

### <a name="groups"></a>组

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 新增了 [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-1.0) |
| 添加项        | v1.0        | 新增了以下组生命周期策略 API：[Create](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-1.0)、[List](/graph/api/grouplifecyclepolicy-list?view=graph-rest-1.0)、[Get](/graph/api/grouplifecyclepolicy-get?view=graph-rest-1.0)、[Update](/graph/api/grouplifecyclepolicy-update?view=graph-rest-1.0)、[Delete](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-1.0)、[Add group](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-1.0)、[Remove group](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-1.0) |
| 新增        | v1.0        | 向 [group](/graph/api/resources/group?view=graph-rest-1.0) 添加了 [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-1.0) 函数 |
| 更改 | v1.0 | 向 [group](/graph/api/resources/group?view=graph-rest-1.0) 添加了 renewedDateTime 属性和 [renew](/graph/api/group-renew?view=graph-rest-1.0) |

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

|更改类型|版本|说明|
|:---|:---|:---|
|更改|beta|向[订阅](/graph/api/resources/subscription?view=graph-rest-beta)资源添加了 **applicationID** 和 **creatorUserID** 属性。 |
|更改|beta|向[订阅](/graph/api/resources/subscription?view=graph-rest-beta) 实体添加了[列表](/graph/api/subscription-list?view=graph-rest-beta)操作。 |

### <a name="identity-and-access--data-policy-operations"></a>身份和访问|数据策略操作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | beta        | 添加了新实体 [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-beta)。 这表示可用于跟踪目的的提交数据策略操作。
| 添加项        | beta        | 在 [users](/graph/api/resources/users?view=graph-rest-beta) 上添加了 [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-beta) 操作。 此操作将提交数据策略操作请求，以导出由 Microsoft 为用户存储的个人数据。 |

### <a name="identity-and-access-directory-apis"></a>标识和访问（目录 API）

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 实体添加了 **onPremisesExtensionAttributes** 复杂类型。 这包含本地 AD 扩展属性 1-15。 |
| 添加        | Beta        | 向 [organization](/graph/api/resources/organization?view=graph-rest-beta) 实体添加了 **privacyProfile** 复杂类型。 |
| 添加项        | v1.0        | 添加了对[还原并永久删除用户和组](/graph/api/resources/directory?view=graph-rest-1.0)的支持。 |

### <a name="identity-and-access--terms-of-use"></a>身份和访问|使用条款

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加了 [agreement](/graph/api/resources/agreement?view=graph-rest-beta) 和 [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta) 资源。 |
| 添加项        | Beta        | 添加了以下 [agreement](/graph/api/resources/agreement?view=graph-rest-beta) API：[Create](/graph/api/greement-post-agreements?view=graph-rest-beta)、[List](/graph/api/agreement-list?view=graph-rest-beta)、[Get](/graph/api/agreement-get?view=graph-rest-beta)、[Update](/graph/api/agreement-update?view=graph-rest-beta)、[Delete](/graph/api/agreement-delete?view=graph-rest-beta)。 |
| 添加项        | Beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 资源添加了 [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta) 关系。 |

### <a name="reports"></a>报告

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Addition|beta|向 [sharePointSiteUsageDetail](/graph/api/resources/sharepointsiteusagedetail?view=graph-rest-beta) 实体添加了 **siteId** 属性。|

### <a name="workbooks-and-charts-excel"></a>工作簿和图表 (Excel)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|更改|v1.0|向 [Excel 表格](/graph/api/resources/table?view=graph-rest-1.0)实体添加了 **legacyId** 属性。 这包含对给定 Excel 表格保持不变的数值标识符（字符串数据类型）。 如果应用程序依赖旧版 Excel 客户端应用程序中使用的旧标识符，这就作为额外元数据提供。 注意：应将 `id` 和 `legacyId` 属性处理为不透明的字符串值，不得在应用程序中将它们解析为其他任何类型。 |


## <a name="february-2018"></a>2018 年 2 月

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|Description|
|:---|:---|:---|
|添加项|beta|新增了实体：<br/>[androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10KioskConfiguration](/graph/api/resources/intune-deviceconfig-windows10kioskconfiguration?view=graph-rest-beta)<br/>[windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)<br/>|
|添加项|beta|新增了复杂类型：<br/>[importedWindowsAutopilotDeviceIdentityState](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate?view=graph-rest-beta)<br/>|
|添加项|beta|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 中添加了 [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) 函数 |
|添加项|beta|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 中添加了 [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) 函数 |
|添加项|beta|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 中添加了 [managedDeviceEnrollmentFailureTrends](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuretrends?view=graph-rest-beta) 函数 |
|添加项|beta|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 中添加了 [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) 函数 |
|添加项|beta|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 中添加了 [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) 函数 |
|更改|beta|从 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体中删除了 **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders** 和 **requireCompanyPortalAppIntegrity** 属性|
|更改|beta|从 [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) 实体中删除了 **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders** 和 **requireCompanyPortalAppIntegrity** 属性|
|更改|beta|从 [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) 实体中删除了 **name**、**modifiedDateTime**、**totalEnrollmentCount** 和 **qrCode** 属性|
|更改|beta|从 [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta) 实体中删除了 **nonEapAuthenticationMethodForEapTtls**、**nonEapAuthenticationMethodForPeap** 和 **enableOuterIdentityPrivacy** 属性|
|更改|beta|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBlockAddingAccounts** 属性|
|更改|beta|从 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **blockCrossProfileCopyPaste** 和 **requireAppVerify** 属性|
|更改|beta|向 [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) 实体添加了 **deviceOwnerManagementEnabled** 属性|
|更改|beta|从 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **requireAppVerify** 属性|
|更改|beta|向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **exemptedAppPackages** 属性|
|更改|beta|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **exemptedAppProtocols** 和 **exemptedAppPackages** 属性|
|更改|beta|向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **exemptedAppProtocols** 属性|
|更改|beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **lastLoggedOnUserId** 属性|
|更改|beta|向 [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) 实体添加了 **isFrameworkFile** 属性|
|更改|beta|向 [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) 实体添加了 **targetedAppManagementLevels** 属性|
|更改|beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **localSecurityOptionsBlockMicrosoftAccounts**、**localSecurityOptionsEnableAdministratorAccount**、**defenderPreventCredentialStealingType**、**defenderProcessCreationType**、**defenderUntrustedUSBProcessType**、**defenderUntrustedExecutableType**、**defenderPasswordProtectedEmailContentExecutionType**、**defenderAdvancedRansomewareProtectionType** 和 **applicationGuardAllowFileSaveOnHost** 属性|
|更改|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **edgeFavoritesListLocation** 和 **edgeBlockEditFavorites** 属性|
|更改|beta|向 [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) 实体添加了 **printerNames**、**defaultPrinterName** 和 **blockAddingNewPrinter** 属性|
|更改|beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **importedWindowsAutopilotDeviceIdentities** 导航属性|
|更改|beta|向 [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta) 复杂类型添加了 **shareAPNSData** 属性|
|更改|beta|从 [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta) 复杂类型中删除了 **collectFullIOSAppInventory** 属性|
|更改|beta|从 [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 复杂类型中删除了 **deviceUsageType** 属性|

### <a name="reports"></a>报告
| 更改类型 | 版本 | 说明                              |
|:------------|:--------|:-----------------------------------------|
| 添加    | Beta    | 向 [userActivationCounts](/graph/api/resources/useractivationcounts?view=graph-rest-beta) 实体添加了 **activatedOnSharedComputer** 属性。|
| 添加项    | Beta    | 向 [office365ActivationsUserCounts](/graph/api/resources/office365activationsusercounts?view=graph-rest-beta) 实体添加了 **sharedComputerActivation** 属性。|

### <a name="tasks-and-plans-planner"></a>任务和计划（规划器）

|更改类型|版本|说明|
|:---|:---|:---|
|添加|Beta|新增了复杂类型：<br/>[plannerPlanContext](/graph/api/resources/plannerplancontext?view=graph-rest-beta)<br/>[plannerPlanContextDetails](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta)<br/>[plannerPlanContextCollection](/graph/api/resources/plannerplancontextcollection?view=graph-rest-beta)<br/>[plannerPlanContextDetailsCollection](/graph/api/resources/plannerplancontextdetailscollection?view=graph-rest-beta)<br/>[plannerFavoritePlanReference](/graph/api/resources/plannerfavoriteplanreference?view=graph-rest-beta)<br/>[plannerRecentPlanReference](/graph/api/resources/plannerrecentplanreference?view=graph-rest-beta)<br/>[plannerFavoritePlanReferenceCollection](/graph/api/resources/plannerfavoriteplanreferencecollection?view=graph-rest-beta)<br/>[plannerRecentPlanReferenceCollection](/graph/api/resources/plannerrecentplanreferencecollection?view=graph-rest-beta)|
|添加项|Beta|向 [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) 实体添加了 `favoritePlanReferences` 和 `recentPlanReferences` 属性。 |
|添加项|Beta|向 [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) 实体添加了 `favoritePlans` 和 `recentPlans` 导航属性。 |
|添加项|Beta|向 [plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) 实体添加了 `contexts` 属性。 |
|添加项|Beta|向 [plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta) 实体添加了 `contextDetails` 属性。 |
|添加项|Beta|添加了 Planner [delta 查询](/graph/api/planneruser-list-delta?view=graph-rest-beta) |


## <a name="january-2018"></a>2018 年 1 月

### <a name="batching"></a>批处理

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|v1.0|添加了 [JSON 批处理](json-batching.md)支持。 内部请求限制设置为 20。|
|更改|Beta|将 [JSON 批处理](json-batching.md)内部请求限制从 5 增加到 20。|

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|添加项|v1.0|添加了新实体：<br/>[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-1.0)<br/>[androidCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidcustomconfiguration?view=graph-rest-1.0)<br/>[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-1.0)<br/>[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-1.0)<br/>[androidManagedAppRegistration](/graph/api/resources/intune-mam-androidmanagedappregistration?view=graph-rest-1.0)<br/>[androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-1.0)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-1.0)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0)<br/>[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-1.0)<br/>[detectedApp](/graph/api/resources/intune-devices-detectedapp?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-1.0)<br/>[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0)<br/>[deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-1.0)<br/>[deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-1.0)<br/>[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-1.0)<br/>[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0)<br/>[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-1.0)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-1.0)<br/>[deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-1.0)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-1.0)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-1.0)<br/>[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-1.0)<br/>[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)<br/>[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-1.0)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-1.0)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-1.0)<br/>[deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-1.0)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-1.0)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-1.0)<br/>[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0)<br/>[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-1.0)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-1.0)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)<br/>[editionUpgradeConfiguration](/graph/api/resources/intune-deviceconfig-editionupgradeconfiguration?view=graph-rest-1.0)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-1.0)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-1.0)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-1.0)<br/>[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-1.0)<br/>[iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-1.0)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-1.0)<br/>[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-1.0)<br/>[iosManagedAppRegistration](/graph/api/resources/intune-mam-iosmanagedappregistration?view=graph-rest-1.0)<br/>[iosStoreApp](/graph/api/resources/intune-apps-iosstoreapp?view=graph-rest-1.0)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-1.0)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-1.0)<br/>[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-1.0)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-1.0)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-1.0)<br/>[localizedNotificationMessage](/graph/api/resources/intune-notification-localizednotificationmessage?view=graph-rest-1.0)<br/>[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0)<br/>[macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-1.0)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-1.0)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-1.0)<br/>[managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-1.0)<br/>[managedApp](/graph/api/resources/intune-apps-managedapp?view=graph-rest-1.0)<br/>[managedAppConfiguration](/graph/api/resources/intune-mam-managedappconfiguration?view=graph-rest-1.0)<br/>[managedAppOperation](/graph/api/resources/intune-mam-managedappoperation?view=graph-rest-1.0)<br/>[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummary](/graph/api/resources/intune-mam-managedapppolicydeploymentsummary?view=graph-rest-1.0)<br/>[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0)<br/>[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0)<br/>[managedAppStatus](/graph/api/resources/intune-mam-managedappstatus?view=graph-rest-1.0)<br/>[managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-1.0)<br/>[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-1.0)<br/>[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-1.0)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-1.0)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-1.0)<br/>[managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-1.0)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-1.0)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-1.0)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-1.0mwindowsinformationprotectionpolicy)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-1.0)<br/>[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-1.0)<br/>[mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-1.0)<br/>[mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-1.0)<br/>[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0)<br/>[mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-1.0)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-1.0)<br/>[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0)<br/>[onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0)<br/>[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-1.0)<br/>[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-1.0)<br/>[roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-1.0)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-1.0)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-1.0)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-1.0)<br/>[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0)<br/>targetedManagedAppPolicyAssignment<br/>[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0)<br/>[telecomExpenseManagementPartner](/graph/api/resources/intune-tem-telecomexpensemanagementpartner?view=graph-rest-1.0)<br/>[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-1.0)<br/>[termsAndConditionsAcceptanceStatus](/graph/api/resources/intune-companyterms-termsandconditionsacceptancestatus?view=graph-rest-1.0)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-1.0)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-1.0)<br/>[webApp](/graph/api/resources/intune-apps-webapp?view=graph-rest-1.0)<br/>[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-1.0)<br/>[windows10CustomConfiguration](/graph/api/resources/intune-deviceconfig-windows10customconfiguration?view=graph-rest-1.0)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-1.0)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-1.0)<br/>[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0)<br/>[windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-1.0)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-1.0)<br/>[windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-1.0)<br/>[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-1.0)<br/>[windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-1.0)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-1.0)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-1.0)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-1.0)<br/>[windowsPhone81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windowsphone81compliancepolicy?view=graph-rest-1.0)<br/>[windowsPhone81CustomConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81customconfiguration?view=graph-rest-1.0)<br/>[windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-1.0)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-1.0)<br/>[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-1.0)<br/>|
|添加|v1.0|新增了复杂类型：<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-1.0)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-1.0)<br/>[androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-1.0)<br/>[androidMobileAppIdentifier](/graph/api/resources/intune-mam-androidmobileappidentifier?view=graph-rest-1.0)<br/>[appListItem](/graph/api/resources/intune-deviceconfig-applistitem?view=graph-rest-1.0)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-1.0)<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-1.0)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-1.0)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devices-deleteuserfromsharedappledeviceactionresult?view=graph-rest-1.0)<br/>[deviceActionResult](/graph/api/resources/intune-devices-deviceactionresult?view=graph-rest-1.0)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-1.0)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-1.0)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-devices-deviceexchangeaccessstatesummary?view=graph-rest-1.0)<br/>[deviceGeoLocation](/graph/api/resources/intune-devices-devicegeolocation?view=graph-rest-1.0)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-1.0)<br/>[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-1.0)<br/>[deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-1.0)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-1.0)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-1.0)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-1.0)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-1.0)<br/>[fileEncryptionInfo](/graph/api/resources/intune-apps-fileencryptioninfo?view=graph-rest-1.0)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-1.0)<br/>[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-1.0)<br/>[iosDeviceType](/graph/api/resources/intune-apps-iosdevicetype?view=graph-rest-1.0)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-1.0)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-1.0)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-1.0)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-1.0)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-1.0)<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-1.0)<br/>[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0)<br/>[iosMobileAppIdentifier](/graph/api/resources/intune-mam-iosmobileappidentifier?view=graph-rest-1.0)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-1.0)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-1.0)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-1.0)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-1.0)<br/>[ipRange](/graph/api/resources/intune-mam-iprange?view=graph-rest-1.0)<br/>[iPv4Range](/graph/api/resources/intune-mam-ipv4range?view=graph-rest-1.0)<br/>[iPv6Range](/graph/api/resources/intune-mam-ipv6range?view=graph-rest-1.0)<br/>[keyValuePair](/graph/api/resources/intune-androidforwork-keyvaluepair?view=graph-rest-1.0)<br/>[locateDeviceActionResult](/graph/api/resources/intune-devices-locatedeviceactionresult?view=graph-rest-1.0)<br/>[managedAppDiagnosticStatus](/graph/api/resources/intune-mam-managedappdiagnosticstatus?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummaryPerApp](/graph/api/resources/intune-mam-managedapppolicydeploymentsummaryperapp?view=graph-rest-1.0)<br/>[mediaContentRatingAustralia](/graph/api/resources/intune-deviceconfig-mediacontentratingaustralia?view=graph-rest-1.0)<br/>[mediaContentRatingCanada](/graph/api/resources/intune-deviceconfig-mediacontentratingcanada?view=graph-rest-1.0)<br/>[mediaContentRatingFrance](/graph/api/resources/intune-deviceconfig-mediacontentratingfrance?view=graph-rest-1.0)<br/>[mediaContentRatingGermany](/graph/api/resources/intune-deviceconfig-mediacontentratinggermany?view=graph-rest-1.0)<br/>[mediaContentRatingIreland](/graph/api/resources/intune-deviceconfig-mediacontentratingireland?view=graph-rest-1.0)<br/>[mediaContentRatingJapan](/graph/api/resources/intune-deviceconfig-mediacontentratingjapan?view=graph-rest-1.0)<br/>[mediaContentRatingNewZealand](/graph/api/resources/intune-deviceconfig-mediacontentratingnewzealand?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedKingdom](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedkingdom?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedStates](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedstates?view=graph-rest-1.0)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-1.0)<br/>[mimeContent](/graph/api/resources/intune-shared-mimecontent?view=graph-rest-1.0)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-1.0)<br/>[mobileAppIdentifier](/graph/api/resources/intune-mam-mobileappidentifier?view=graph-rest-1.0)<br/>[omaSetting](/graph/api/resources/intune-deviceconfig-omasetting?view=graph-rest-1.0)<br/>[omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-1.0)<br/>[omaSettingBoolean](/graph/api/resources/intune-deviceconfig-omasettingboolean?view=graph-rest-1.0)<br/>[omaSettingDateTime](/graph/api/resources/intune-deviceconfig-omasettingdatetime?view=graph-rest-1.0)<br/>[omaSettingFloatingPoint](/graph/api/resources/intune-deviceconfig-omasettingfloatingpoint?view=graph-rest-1.0)<br/>[omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-1.0)<br/>[omaSettingString](/graph/api/resources/intune-deviceconfig-omasettingstring?view=graph-rest-1.0)<br/>[omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-1.0)<br/>[proxiedDomain](/graph/api/resources/intune-mam-proxieddomain?view=graph-rest-1.0)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-1.0)<br/>[resetPasscodeActionResult](/graph/api/resources/intune-devices-resetpasscodeactionresult?view=graph-rest-1.0)<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-1.0)<br/>[rgbColor](/graph/api/resources/intune-onboarding-rgbcolor?view=graph-rest-1.0)<br/>[rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-1.0)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-1.0)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-1.0)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-1.0)<br/>[vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-1.0)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-1.0)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-1.0)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-1.0)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-1.0)<br/>[windowsDeviceAzureADAccount](/graph/api/resources/intune-devices-windowsdeviceazureadaccount?view=graph-rest-1.0)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-1.0)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-1.0)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-1.0)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-1.0)<br/>[windowsUpdateActiveHoursInstall](/graph/api/resources/intune-deviceconfig-windowsupdateactivehoursinstall?view=graph-rest-1.0)<br/>[windowsUpdateInstallScheduleType](/graph/api/resources/intune-deviceconfig-windowsupdateinstallscheduletype?view=graph-rest-1.0)<br/>[windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-1.0)<br/>|
|添加项|v1.0|在 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) 上添加了 [commit](/graph/api/intune-apps-mobileappcontentfile-commit?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) 上添加了 [renewUpload](/graph/api/intune-apps-mobileappcontentfile-renewupload?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [retire](/graph/api/intune-devices-manageddevice-retire?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [resetPasscode](/graph/api/intune-devices-manageddevice-resetpasscode?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [remoteLock](/graph/api/intune-devices-manageddevice-remotelock?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [disableLostMode](/graph/api/intune-devices-manageddevice-disablelostmode?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [locateDevice](/graph/api/intune-devices-manageddevice-locatedevice?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [bypassActivationLock](/graph/api/intune-devices-manageddevice-bypassactivationlock?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [rebootNow](/graph/api/intune-devices-manageddevice-rebootnow?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-1.0) 操作 |
|添加|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-1.0) 操作 |
|Addition|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) 上添加了 [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) 上添加了 [removeAllDevicesFromManagement](/graph/api/intune-devices-user-removealldevicesfrommanagement?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-1.0) 操作 |
|Addition|v1.0|在 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) 上添加了 [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0) 上添加了 [setMobileDeviceManagementAuthority](/graph/api/intune-onboarding-organization-setmobiledevicemanagementauthority?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0) 上添加了 [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) 上添加了 [sync](/graph/api/intune-onboarding-devicemanagementexchangeconnector-sync?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) 上添加了 [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-mam-targetedmanagedappprotection-assign?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-mam-targetedmanagedappconfiguration-assign?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-mam-windowsinformationprotection-assign?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0) 上添加了 [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0) 上添加了 [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) 上添加了 [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) 上添加了 [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0) 上添加了 [sendTestMessage](/graph/api/intune-notification-notificationmessagetemplate-sendtestmessage?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0) 上添加了 [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) 上添加了 [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) 上添加了 [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-1.0) 操作 |
|添加项|v1.0|在 [applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0) 上添加了 [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-1.0) 函数 |
|添加项|v1.0|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) 上添加了 [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-1.0) 函数 |
|添加项|v1.0|在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) 上添加了 [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-1.0) 函数 |
|添加项|v1.0|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) 上添加了 [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-1.0) 函数 |
|添加项|v1.0|在 [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0) 集合上添加了 **getUserIdsWithFlaggedAppRegistration** 函数 |
|添加项|v1.0|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) 上添加了 [getManagedAppDiagnosticStatuses](/graph/api/intune-mam-user-getmanagedappdiagnosticstatuses?view=graph-rest-1.0) 函数 |
|添加项|v1.0|在 [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) 上添加了 [getManagedAppPolicies](/graph/api/intune-mam-user-getmanagedapppolicies?view=graph-rest-1.0) 函数 |
|添加项|v1.0|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) 上添加了 [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-1.0) 函数 |
|更改|v1.0|向 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0) 实体添加了 **mobileDeviceManagementAuthority** 属性|
|更改|v1.0|向 [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) 实体添加了 **deviceEnrollmentLimit** 属性|
|更改|v1.0|向 [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) 实体添加了 **managedDevices**、**managedAppRegistrations** 和 **deviceManagementTroubleshootingEvents** 导航属性|
|||
|添加项|Beta|添加了新实体：<br/>[deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-beta)<br/>|
|添加项|Beta|新增了复杂类型：<br/>[revokeAppleVppLicensesActionResult](/graph/api/resources/intune-devices-revokeapplevpplicensesactionresult?view=graph-rest-beta)<br/>[vppTokenRevokeLicensesActionResult](/graph/api/resources/intune-onboarding-vpptokenrevokelicensesactionresult?view=graph-rest-beta)<br/>|
|添加项|Beta|在 [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) 上添加了 [revokeToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-devices-devicemanagementscript-assign?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [revokeAppleVppLicenses](/graph/api/intune-devices-manageddevice-revokeapplevpplicenses?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) 操作 |
|Addition|Beta|对 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) 新增了 [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) 操作 |
|添加|Beta|在 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 上添加了 [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) 操作 |
|Addition|Beta|在 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 上添加了 [getEffectiveDeviceEnrollmentConfigurations](/graph/api/intune-onboarding-user-geteffectivedeviceenrollmentconfigurations?view=graph-rest-beta) 函数 |
|删除|Beta|删除了以下实体：<br/>**appReportingOverviewStatus**<br/>**complianceSettingStateSummary**<br/>**deviceConfigurationUserStateSummary**<br/>**eBookGroupAssignment**<br/>**eBookVppGroupAssignment**<br/>**mobileAppGroupAssignment**<br/>**mobileAppVppGroupAssignment**<br/>|
|删除|Beta|删除了以下复杂类型：<br/>**androidForWorkAppConfigurationExample**<br/>**androidForWorkAppConfigurationExampleJson**<br/>**appInstallationFailure**<br/>**appsComplianceListItem**<br/>**defaultDeviceEnrollmentRestrictions**<br/>**defaultDeviceEnrollmentWindowsHelloForBusinessSettings**<br/>**deviceEnrollmentPlatformRestrictions**<br/>|
|更改|Beta 版本|向 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体添加了 **securityRequireVerifyApps**、**securityRequireSafetyNetAttestationBasicIntegrity**、**securityRequireSafetyNetAttestationCertifiedDevice**、**securityRequireGooglePlayServices**、**securityRequireUpToDateSecurityProviders** 和 **securityRequireCompanyPortalAppIntegrity** 属性|
|更改|Beta 版本|向 [androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta) 实体添加了 **packageId** 属性|
|更改|Beta 版本|更改了 [androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta) 实体上以下属性的类型：<br/>**exampleJson** 从 [androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta) 改为 Binary<br/>|
|更改|Beta 版本|向 [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) 实体添加了 **securityRequireVerifyApps**、**securityRequireSafetyNetAttestationBasicIntegrity**、**securityRequireSafetyNetAttestationCertifiedDevice**、**securityRequireGooglePlayServices**、**securityRequireUpToDateSecurityProviders** 和 **securityRequireCompanyPortalAppIntegrity** 属性|
|更改|Beta 版本|向 [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) 实体添加了 **displayName**、**lastModifiedDateTime**、**enrolledDeviceCount**、**qrCodeContent** 和 **qrCodeImage** 属性|
|更改|Beta 版本|从 [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) 实体中删除了 **isTokenActive** 属性|
|更改|Beta 版本|向 [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **innerAuthenticationProtocolForEapTtls**、**innerAuthenticationProtocolForPeap** 和 **outerIdentityPrivacyTemporaryValue** 属性|
|更改|Beta 版本|向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfileBlockCrossProfileCopyPaste** 和 **securityRequireVerifyApps** 属性|
|更改|Beta 版本|向 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **securityRequireVerifyApps** 属性|
|更改|Beta 版本|向 [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta) 实体添加了 **packageId** 和 **identityVersion** 属性|
|更改|Beta 版本|向 [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta) 实体添加了 **packageId** 属性|
|更改|Beta 版本|向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **faceIdBlocked** 属性|
|更改|Beta 版本|向 [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta) 实体添加了 **members** 属性|
|更改|Beta 版本|向 [deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta) 实体添加了 **macOSRestriction** 属性|
|“更改”|Beta 版本|向 [deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta) 实体添加了 **whenPartnerDevicesWillBeRemovedDateTime** 和 **whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime** 属性|
|更改|Beta 版本|更改了 [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) 实体以下属性的类型：<br/>**scriptContent**从 String 改为 Binary<br/>|
|更改|Beta 版本|向 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体添加了 **smimeEnablePerMessageSwitch** 属性|
|更改|Beta 版本|向 [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta) 实体添加了 **identityVersion** 属性|
|更改|Beta 版本|向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **faceIdBlocked** 属性|
|更改|Beta 版本|向 [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta) 实体添加了 **packageId** 和 **identityVersion** 属性|
|更改|Beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **azureADDeviceId** 和 **remoteAssistanceSessionErrorDetails** 属性|
|更改|Beta|从 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 实体删除了 **legacyAppConfiguration** 属性|
|更改|Beta|向 [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta) 实体添加了 **identityVersion** 属性|
|更改|Beta|从 [managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta) 实体删除了 **identityVersion** 属性|
|更改|Beta|向 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 实体添加了 **publishingState** 属性|
|更改|Beta|向 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) 实体添加了 **installState** 属性|
|更改|Beta|从 [mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-beta) 实体删除了 **identityVersion** 属性|
|更改|Beta|向 [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta) 实体添加了 **allowPartnerToCollectIOSApplicationMetadata** 属性|
|更改|Beta|从 [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) 实体删除了 **members** 属性|
|更改|Beta|向 [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta) 实体添加了 **lastModifiedDateTime** 属性。|
|更改|Beta|向 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 实体添加了 **deviceThreatProtectionEnabled** 和 **deviceThreatProtectionRequiredSecurityLevel** 属性|
|更改|Beta|从 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 实体删除了 **minimumUpdateAutoInstallClassification** 属性|
|更改|Beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **privacyBlockPublishUserActivities** 和 **privacyBlockActivityFeed** 属性|
|更改|Beta|向 [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) 实体添加了 **configurationAccountType** 属性|
|更改|Beta|从 [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) 实体删除了 **trustedNetworkDomains** 属性|
|更改|Beta|从 [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta) 实体删除了 **minimumUpdateAutoInstallClassification** 属性|
|更改|Beta|向 [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta) 实体添加了 **identityVersion** 属性|
|更改|Beta|向 [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta) 实体添加了 **daysWithoutContactBeforeUnenroll** 属性|
|更改|Beta|向 [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) 实体添加了 **identityVersion** 属性|
|更改|Beta|向 [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) 实体添加了 **identityVersion** 属性|
|更改|Beta|向 [windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta) 实体添加了 **identityVersion** 属性|
|更改|Beta|向 [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) 实体添加了 **identityVersion** 属性|
|更改|Beta|向 [activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta) 实体添加了 **domainJoinConfiguration** 导航属性|
|更改|Beta|从 [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) 实体删除了 **notificationMessageTemplate** 导航属性|
|更改|Beta|从 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 实体删除了 **groupAssignments** 导航属性|
|更改|Beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **windowsInformationProtectionNetworkLearningSummaries** 导航属性|
|更改|Beta|从 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体删除了 **deviceConfigurationUserStateSummaries** 导航属性|
|更改|Beta|更改了 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体上以下属性的类型：<br/>**roleAssignments** 从 [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) 集合更改为 [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta) 集合<br/>|
|更改|Beta|向 [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) 实体添加了 **assignments** 导航属性|
|更改|Beta|向 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体添加了 **smimeEncryptionCertificate** 导航属性|
|更改|Beta|更改了 [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) 实体以下属性的类型：<br/>**smimeSigningCertificate** 从 [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) 更改为 [iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta)<br/>|
|更改|Beta|从 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 实体删除了 **vppToken** 导航属性|
|更改|Beta|从 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) 实体删除了 **groupAssignments** 导航属性|
|更改|Beta 版本|从 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 实体删除了 **groupAssignments** 导航属性|
|更改|Beta 版本|从 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 实体删除了 **depOnboardingSettings** 和 **appleVolumePurchaseProgramTokens** 导航属性|
|更改|Beta 版本|向 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 实体添加了 **deviceEnrollmentConfigurations** 导航属性|
|更改|Beta 版本|从 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型删除了 **windowsCommercialId** 和 **windowsCommercialIdLastModifiedTime** 属性|
|更改|Beta 版本|向 [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) 复杂类型添加了 **showDisplayNameNextToLogo** 属性|
|更改|Beta 版本|向 [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 复杂类型添加了 **deviceUsageType** 属性|
|更改|Beta 版本|向 [vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-beta) 复杂类型添加了 **supportsUserLicensing** 和 **supportsDeviceLicensing** 属性|
|更改|Beta 版本|从 [vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta) 复杂类型中删除了 **actionMessage** 属性|

### <a name="education"></a>教育

|更改类型|版本|说明|
|:---|:---|:---|
|添加|Beta|添加了其他导航属性并改进对[名单 API](/graph/api/resources/education-overview?view=graph-rest-beta) 的筛选支持。|

### <a name="reports"></a>报告
| 更改类型 | 版本 | 说明                              |
|:------------|:--------|:-----------------------------------------|
| 添加项    | v1.0    | 新增了以下 API：<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-1.0)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-1.0)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-1.0) |

## <a name="december-2017"></a>2017 年 12 月

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

|更改类型|版本|说明|
|:---|:---|:---|
|添加|Beta|新增了实体：<br/>[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>|
|添加项|Beta|新增了复杂类型：<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-beta)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-beta)<br/>[vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta)<br/>[windowsDeviceAADAccount](/graph/api/resources/intune-devices-windowsdeviceaadaccount?view=graph-rest-beta)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-beta)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-beta)<br/>|
|添加项|Beta|对 [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) 新增了 [revokeTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketokens?view=graph-rest-beta) 操作 |
|添加项|Beta|对 [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) 新增了 [createToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-createtoken?view=graph-rest-beta) 操作 |
|添加项|Beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 新增了 [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) 操作 |
|Addition|Beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 新增了 [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-beta) 操作 |
|Addition|Beta|对 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) 新增了 [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) 操作 |
|添加项|Beta|对 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 集合新增了 [getDevicePasscode](/graph/api/intune-deviceconfig-devicecompliancepolicy-getdevicepasscode?view=graph-rest-beta) 函数 |
|添加项|Beta|在 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 上添加了 [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-beta) 函数 |
|删除|Beta|删除了以下实体：<br/>**windowsStoreForBusinessApp**<br/>|
|删除|Beta|删除了以下复杂类型：<br/>**windowsStoreForBusinessAppAssignmentSettings**<br/>|
|更改|Beta 版本|向 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **dateAndTimeBlockChanges** 属性|
|更改|Beta|从 [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) 实体中删除了 **enableAuthenticationViaCompanyPortal** 属性|
|更改|Beta|从 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体中删除了 **windowsStoreForBusinessLastSuccessfulSyncDateTime**、**isEnabledForWindowsStoreForBusiness**、**windowsStoreForBusinessLanguage** 和 **windowsStoreForBusinessLastCompletedApplicationSyncTime** 属性|
|更改|Beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **maximumDepTokens** 和 **intuneAccountId** 属性|
|更改|Beta|向 [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) 实体添加了 **enableAuthenticationViaCompanyPortal** 属性|
|更改|Beta|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **managedDeviceName** 和 **partnerReportedThreatState** 属性|
|更改|Beta|向 [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) 实体添加了 **installProgressDisplayLevel** 属性|
|更改|Beta|向 [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) 实体添加了 **resourceScopes** 属性|
|更改|Beta|向 [roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-beta) 实体添加了 **rolePermissions** 和 **isBuiltIn** 属性|
|更改|Beta|向 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) 实体添加了 **tokenActionResults** 属性|
|更改|Beta|向 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 实体添加了 **minimumUpdateAutoInstallClassification** 属性|
|更改|Beta|向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **defenderSecurityCenterDisableAppBrowserUI**、**defenderSecurityCenterDisableFamilyUI**、**defenderSecurityCenterDisableHealthUI**、**defenderSecurityCenterDisableNetworkUI**、**defenderSecurityCenterDisableVirusUI**、**defenderSecurityCenterOrganizationDisplayName**、**defenderSecurityCenterHelpEmail**、**defenderSecurityCenterHelpPhone**、**defenderSecurityCenterHelpURL**、**defenderSecurityCenterNotificationsFromApp**、**defenderSecurityCenterITContactDisplay** 和 **applicationGuardAllowVirtualGPU** 属性|
|更改|Beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **enableAutomaticRedeployment** 和 **authenticationAllowFIDODevice** 属性|
|更改|Beta|向 [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) 实体添加了 **trustedNetworkDomains** 属性|
|更改|Beta|向 [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta) 实体添加了 **minimumUpdateAutoInstallClassification** 属性|
|更改|Beta|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **androidForWorkEnrollmentProfiles** 导航属性|
|更改|Beta|向 [deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta) 复杂类型添加了 **healthAttestationSupportedStatus** 属性|
|更改|Beta|向 [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta) 复杂类型添加了 **tpmSpecificationVersion**、**operatingSystemEdition**、**deviceFullQualifiedDomainName**、**deviceGuardVirtualizationBasedSecurityHardwareRequirementState**、**deviceGuardVirtualizationBasedSecurityState** 和 **deviceGuardLocalSystemAuthorityCredentialGuardState** 属性|
|更改|Beta|向 [iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta) 复杂类型添加了 **vpnConfigurationId** 属性|
|更改|Beta|向 [rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-beta) 复杂类型添加了 **resourceActions** 属性|

### <a name="reports"></a>报告
| 更改类型 | 版本 | 说明                              |
|:------------|:--------|:-----------------------------------------|
| 添加项    | v1.0    | 新增了以下 API：<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-1.0)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-1.0)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-1.0)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-1.0)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-1.0)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-1.0)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-1.0)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-1.0)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-1.0)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-1.0)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-1.0)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-1.0)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-1.0)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-1.0)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-1.0)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-1.0)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-1.0)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-1.0)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-1.0)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-1.0)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-1.0)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-1.0)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-1.0)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-1.0)。|
| Addition    | Beta    | 新增了以下 API：<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-beta)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-beta) |

### <a name="track-changes"></a>跟踪更改

| 更改类型 | 版本 | 说明                              |
|:------------|:--------|:-----------------------------------------|
| 更改      | v1.0    | 向[用户](/graph/api/user-delta?view=graph-rest-1.0)和[组](/graph/api/group-delta?view=graph-rest-1.0) 添加可选的增量查询筛选功能。 |


## <a name="november-2017"></a>2017 年 11 月

### <a name="change-notifications-webhooks"></a>更改通知（Webhook）

| 更改类型 | 版本 | 说明                              |
|:------------|:--------|:-----------------------------------------|
| 重大更改 | Beta 和 v1.0 | 缩短了驱动器根项的 [Webhook](/graph/api/resources/webhooks?view=graph-rest-1.0) [最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)。 新值是支持的驱动器根项最长订阅有效期。 |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|Description|
|:---|:---|:---|
|添加|Beta|新增了实体：<br/>[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta)<br/>[deviceSetupConfiguration](/graph/api/resources/intune-deviceconfig-devicesetupconfiguration?view=graph-rest-beta)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-beta)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-beta)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta)<br/>[ndesConnector](/graph/api/resources/intune-deviceconfig-ndesconnector?view=graph-rest-beta)<br/>|
|添加项|Beta|新增了复杂类型：<br/>[auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)<br/>[auditProperty](/graph/api/resources/intune-auditing-auditproperty?view=graph-rest-beta)<br/>[auditResource](/graph/api/resources/intune-auditing-auditresource?view=graph-rest-beta)<br/>[bulkManagedDeviceActionResult](/graph/api/resources/intune-devices-bulkmanageddeviceactionresult?view=graph-rest-beta)<br/>[deviceProtectionOverview](/graph/api/resources/intune-devices-deviceprotectionoverview?view=graph-rest-beta)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>[operatingSystemVersionRange](/graph/api/resources/intune-deviceconfig-operatingsystemversionrange?view=graph-rest-beta)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-beta)<br/>|
|添加项|Beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 集合新增了 executeAction 操作 |
|添加项|Beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 新增了 [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) 操作 |
|添加项|Beta|对 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 新增了 [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-beta) 操作 |
|添加项|Beta|对 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 新增了 [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-beta) 操作 |
|添加项|Beta|对 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 新增了 [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-beta) 操作 |
|添加项|Beta|对 [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) 新增了 setDefaultProfile 操作 |
|添加项|Beta|对 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 新增了 shareForSchoolDataSyncService 操作 |
|添加项|Beta|对 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 新增了 unshareForSchoolDataSyncService 操作 |
|添加项|Beta|对 [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) 集合新增了 getAuditCategories 函数 |
|添加项|Beta|对 [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) 集合新增了 getAuditActivityTypes 函数 |
|删除|Beta|删除了以下实体：<br/>**mobileAppIdentifierDeployment**<br/>|
|删除|Beta|删除了以下复杂类型：<br/>**windowsInformationProtectionCloudResource**<br/>**windowsInformationProtectionCloudResourceCollection**<br/>|
|更改|Beta|更改了 [androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta) 实体的以下属性：<br/>将 **passcode** 从必需属性更改为可选属性<br/>|
|更改|Beta 版本|向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **microsoftStoreForBusinessLastSuccessfulSyncDateTime**、**isEnabledForMicrosoftStoreForBusiness**、**microsoftStoreForBusinessLanguage** 和 **microsoftStoreForBusinessLastCompletedApplicationSyncTime** 属性|
|更改|Beta 版本|向 [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta) 实体添加了 **target** 属性|
|更改|Beta 版本|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceProtectionOverview** 属性|
|更改|Beta 版本|向 [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) 实体添加了 **exchangeAlias** 和 **exchangeOrganization** 属性|
|更改|Beta 版本|向 [managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-beta) 实体添加了 **appStoreUrl** 和 **minimumSupportedOperatingSystem** 属性|
|更改|Beta 版本|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **remoteAssistanceSessionErrorString** 属性|
|更改|Beta 版本|向 [managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-beta) 实体添加了 **appStoreUrl**、**applicableDeviceType** 和 **minimumSupportedOperatingSystem** 属性|
|更改|Beta 版本|向 [mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta) 实体添加了 **notApplicableDeviceCount**、**pendingInstallDeviceCount**、**notApplicableUserCount** 和 **pendingInstallUserCount** 属性|
|更改|Beta|从 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体中删除了 **targetedSecurityGroupIds** 和 **targetedSecurityGroupsCount** 属性|
|更改|Beta 版本|从 [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) 实体中删除了 **targetedSecurityGroupsCount** 和 **targetedSecurityGroupIds** 属性|
|更改|Beta 版本|向 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 实体添加了 **validOperatingSystemBuildRanges** 属性|
|更改|Beta 版本|向 [windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-beta) 实体添加了 **activeFirewallRequired**、**uacRequired** 和 **validOperatingSystemBuildRanges** 属性|
|更改|Beta 版本|向 [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta) 实体添加了 **enableExpeditedTelemetryReporting** 属性|
|更改|Beta 版本|从 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 实体中删除了 **allowedApps**、**enterpriseCloudResources** 和 **targetedSecurityGroupIds** 属性|
|更改|Beta 版本|向 [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) 实体添加了 **ignoreVersionDetection** 属性|
|更改|Beta 版本|从 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体中删除了 **mobileAppIdentifierDeployments** 导航属性|
|更改|Beta 版本|从 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体中删除了 **mobileAppIdentifierDeployments** 导航属性|
|更改|Beta 版本|向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 实体添加了 **assignments** 导航属性|
|更改|Beta 版本|从 [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta) 实体中删除了 **deviceConfiguration** 导航属性|
|更改|Beta 版本|向 [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) 实体添加了 **deviceConfiguration** 导航属性|
|更改|Beta 版本|向 [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceSetupConfigurations**、**ndesConnectors**、**exchangeOnPremisesPolicies**、**conditionalAccessSettings**、**auditEvents** 和 **troubleshootingEvents** 导航属性|
|更改|Beta 版本|从 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体中删除了 **mobileAppIdentifierDeployments** 导航属性|
|更改|Beta 版本|向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **windowsProtectionState** 导航属性|
|更改|Beta 版本|从 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体中删除了 **mobileAppIdentifierDeployments** 和 **targetedSecurityGroups** 导航属性|
|更改|Beta 版本|从 [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) 实体中删除了 **targetedSecurityGroups** 导航属性|
|更改|Beta 版本|向 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 实体添加了 **deviceManagementTroubleshootingEvents** 导航属性|
|更改|Beta 版本|从 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 实体中删除了 **allowedAppLockerFiles** 导航属性|
|更改|Beta 版本|从 [windowsManagedDevice](/graph/api/resources/intune-devices-windowsmanageddevice?view=graph-rest-beta) 实体中删除了 **windowsProtectionState** 导航属性|
|更改|Beta|向 [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta) 复杂类型添加了 **v11_0** 属性|
|更改项|Beta|向 [windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta) 复杂类型添加了 **denied** 属性|

### <a name="education"></a>教育

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|新增了对教育版方案的支持，包括添加了以下资源：<br/>[学校](/graph/api/resources/educationschool?view=graph-rest-beta)<br/>[课程](/graph/api/resources/educationclass?view=graph-rest-beta)<br/>[用户](/graph/api/resources/educationuser?view=graph-rest-beta)<br/>[作业](/graph/api/resources/educationassignment?view=graph-rest-beta)<br/>[提交](/graph/api/resources/educationsubmission?view=graph-rest-beta)<br/>请参阅资源主题，详细了解可用方法。|

### <a name="identity-and-access--synchronization"></a>身份和访问|同步

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加项    | Beta    | 新增了对 Azure AD 标识同步的支持，包括添加了以下资源：<br/>[作业](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)<br/>[架构](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)<br/>[模板](/graph/api/resources/synchronization-synchronizationtemplate?view=graph-rest-beta)<br/>请参阅资源主题，详细了解可用方法。|

### <a name="reports"></a>报告
| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加项    | Beta    | 增加了对以下 API 的 JSON 支持：<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta). |


## <a name="october-2017"></a>2017 年 10 月

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)
|更改类型|版本|说明|
|:---|:---|:---|
|添加|Beta|添加了新实体：<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfigurationAssignment](/graph/api/resources/intune-apps-ioslobappprovisioningconfigurationassignment?view=graph-rest-beta)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-beta)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-beta)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-beta)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-beta)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)<br/>[windows10PFXImportCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pfximportcertificateprofile?view=graph-rest-beta)<br/>[windowsAssignedAccessProfile](/graph/api/resources/intune-deviceconfig-windowsassignedaccessprofile?view=graph-rest-beta)<br/>[windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta)<br/>|
|添加项|Beta|添加了复杂类型：<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta)<br/>[iosSingleSignOnSettings](/graph/api/resources/intune-deviceconfig-iossinglesignonsettings?view=graph-rest-beta)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-beta)<br/>[proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-beta)<br/>[windowsStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-windowsstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>|
|添加项|Beta|在 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) 操作 |
|添加|Beta|在 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 上添加了 [assignedAccessMultiModeProfiles](/graph/api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) 上添加了 [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) 上添加了 [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 上添加了 [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 上添加了 [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-beta) 操作 |
|添加项|Beta|在 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) 操作 |
|删除项|Beta|删除了以下实体：<br/>**cloudPkiSubscription**<br/>|
|删除项|Beta|删除了以下复杂类型：<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|更改|Beta 版本|将 **gracePeriodInMinutes** 属性添加到 [androidDeviceComplianceLocalActionBase](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionbase?view=graph-rest-beta) 实体|
|更改|Beta 版本|将 **enableSplitTunneling** 属性从 [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta) 实体删除|
|更改|Beta 版本|将 **versionName** 和 **versionCode** 属性添加到 [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta) 实体|
|更改|Beta 版本|将 **minimumRequiredPatchVersion** 和 **minimumWarningPatchVersion** 属性添加到 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体|
|更改|Beta 版本|将 **minimumRequiredPatchVersion** 和 **minimumWarningPatchVersion** 属性添加到 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体|
|更改|Beta 版本|将 **target** 属性添加到 [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta) 实体|
|更改|Beta 版本|将 **singleSignOnSettings** 属性添加到 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) 实体|
|更改|Beta 版本|将 **versionNumber** 和 **buildNumber** 属性添加到 [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta) 实体|
|更改内容|Beta|将 **bundleId** 属性添加到 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 实体|
|更改内容|Beta|向 [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta) 实体添加了 **preSharedKey** 属性|
|更改|Beta|将 **versionName** 和 **versionCode** 属性添加到 [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta) 实体|
|更改内容|Beta|将 **periodBeforePinReset** 属性添加到 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体|
|更改|Beta|将 **subscriberCarrier**、**meid**、**totalStorageSpaceInBytes** 和 **freeStorageSpaceInBytes** 属性添加到 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体|
|更改|Beta|将 **enrollmentType** 属性从 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体删除|
|更改|Beta|将 **versionNumber** 和 **buildNumber** 属性添加到 [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta) 实体|
|更改|Beta|将 **displayVersion** 属性添加到 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) 实体|
|更改|Beta|将 **defaultDeviceEnrollmentRestrictions**、**defaultDeviceEnrollmentWindowsHelloForBusinessSettings** 和 **defaultDeviceEnrollmentLimit** 属性从 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 实体删除|
|更改|Beta|将 **isAssigned** 属性添加到 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体|
|更改|Beta|将 **isAssigned** 属性添加到 [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) 实体|
|更改|Beta|将 **activeFirewallRequired**、**uacRequired**、**defenderEnabled**、**defenderVersion**、**signatureOutOfDate** 和 **rtpEnabled** 属性添加到 [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) 实体|
|更改|Beta|将 **assignedAccessSingleModeUserName**、**assignedAccessSingleModeAppUserModelId**、**microsoftAccountSignInAssistantSettings**、**authenticationAllowSecondaryDevice**、**cryptographyAllowFipsAlgorithmPolicy**、**securityBlockAzureADJoinedDevicesAutoEncryption**、**systemTelemetryProxyServer**、**inkWorkspaceAccess**、**inkWorkspaceBlockSuggestedApps**、**defenderCloudBlockLevel** 和 **defenderCloudExtendedTimeout** 属性添加到 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体|
|更改|Beta|将 **protectedApps**、**enterpriseProxiedDomains** 和 **isAssigned** 属性添加到 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 实体|
|更改|Beta|将 **productVersion** 属性添加到 [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) 实体|
|更改|Beta|将 **apps** 导航属性添加到 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体|
|更改|Beta|将 **apps** 导航属性添加到 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体|
|更改|Beta|将 **vppTokens** 导航属性添加到 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体|
|更改|Beta|将 **assignments** 导航属性添加到 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 实体|
|更改|Beta|将 **deviceCompliancePolicy** 导航属性从 [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta) 实体删除|
|更改|Beta|将 **deviceCompliancePolicy** 导航属性添加到 [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta) 实体|
|更改|Beta|将 **identityCertificateForClientAuthentication** 导航属性添加到 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) 实体|
|更改|Beta|将 **assignments** 导航属性添加到 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体|
|更改|Beta|将 **apps** 导航属性添加到 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体|
|更改内容|Beta|将 **assignments** 导航属性添加到 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 实体|
|更改|Beta|将 **assignments** 导航属性添加到 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) 实体|
|更改|Beta|将 **assignments** 导航属性添加到 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 实体|
|更改|Beta|将 **apps** 导航属性添加到 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体|
|更改|Beta|将 **assignments** 导航属性添加到 [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta) 实体|
|更改|Beta|将 **assignedAccessMultiModeProfiles** 导航属性添加到 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体|
|更改|Beta|将 **protectedAppLockerFiles** 导航属性添加到 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 实体|
|更改|Beta|将 **port** 和 **forceTls** 属性添加到 [airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta) 复杂类型|
|更改|Beta|更改了 [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 复杂类型上以下属性的类型：<br/>**errorCode**（从 Int32 更改为 Int64）<br/>|
|更改|Beta|更改了 [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 复杂类型上以下属性的类型：<br/>**errorCode**（从 Int32 更改为 Int64）<br/>|
|更改|Beta|更改了 [windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta) 复杂类型上以下属性的类型：<br/>**enterpriseCloudResources** 从 [windowsNetworkIsolationCloudResourceCollection](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationcloudresourcecollection?view=graph-rest-beta) 更改为 [proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta) 集合<br/>**enterpriseInternalProxyServers** 从 windowsNetworkIsolationResourceCollection 更改为 String 集合<br/>**enterpriseIPRanges** 从 [windowsNetworkIsolationIPRangeCollection](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta) 更改为 ipRange 集合<br/>**enterpriseNetworkDomainNames** 从 windowsNetworkIsolationResourceCollection 更改为 String 集合<br/>**enterpriseProxyServers** 从 windowsNetworkIsolationResourceCollection 更改为 String 集合<br/>**neutralDomainResources** 从 windowsNetworkIsolationResourceCollection 更改为 String 集合<br/>|

### <a name="identity-and-access-azure-ad"></a>身份和访问 (Azure AD)

| 更改类型 | 版本 | Description                              |
| :---------- | :------ | :--------------------------------------- |
|添加项|Beta|添加了 [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-beta) 实体，以及 [create](/graph/api/identityprovider-post-identityproviders?view=graph-rest-beta)、[list](/graph/api/identityprovider-list?view=graph-rest-beta)、[get](/graph/api/identityprovider-get?view=graph-rest-beta)、[update](/graph/api/identityprovider-update?view=graph-rest-beta) 和 [delete](/graph/api/identityprovider-delete?view=graph-rest-beta) 操作。|

### <a name="mail-outlook"></a>邮件 (Outlook)

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 更改          | v1.0 和 beta | 在用户已与登录用户共享邮件文件夹，或已将其邮箱委派给登录用户时，此行为增强功能可获取该共享邮件文件夹或其邮件内容。 在这种情况下，只要登录 用户已经向应用提供了委派权限，应用即可指定该用户的 ID 或用户主体名称来[获取该共享邮件文件夹](/graph/api/mailfolder-get?view=graph-rest-1.0)，或者[获取该共享日历中的邮件](/graph/api/user-list-messages?view=graph-rest-1.0)。 |

### <a name="reports"></a>报告
| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| Change      | Beta    | 添加了 [getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)、[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta) 和 [getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) API。 这些 API 取代了 EmailActivity API。 |
| Change      | Beta    | 添加了 [getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)、[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)、[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta) 和 [getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta) API。 这些 API 取代了 EmailAppUsage API。 |
| Change      | Beta    | 添加了 [getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)、[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)、[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta) 和 [getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta) API。 这些 API 取代了 MailboxUsage API。 |
| Change      | Beta    | 添加了 [getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)、[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta) 和 [getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta) API。 这些 API 取代了 Office365Activations API。 |
| Change      | Beta    | 添加了 [getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)、[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta) 和 [getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta) API。 这些 API 取代了 Office365ActiveUser API。 |
| Change      | Beta    | 添加了 [getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)、[getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)、[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)、[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta) 和 [getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta) API。 这些 API 取代了 Office365GroupsActivity API。 |
| Change      | Beta    | 添加了 [getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)、[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta) 和 [getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta) API。 这些 API 取代了 OneDriveActivity API。 |
| Change      | Beta    | 添加了 [getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)、[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)、[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta) 和 [getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta) API。 这些 API 取代了 OneDriveUsage API。 |
| Change      | Beta    | 添加了 [getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)、[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)、[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta) 和 [getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta) API。 这些 API 取代了 SharePointActivity API。 |
| Change      | Beta    | 添加了 [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)、[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)、[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)、[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta) 和 [getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta) API。 这些 API 取代了 SharePointSiteUsage API。 |
| Change      | Beta    | 添加了 [getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)、[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta) 和 [getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta) API。 这些 API 取代了 SfbActivity API。 |
| Change      | Beta    | 添加了 [getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)、[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta) 和 [getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta) API。 这些 API 取代了 SfbDeviceUsage API。 |
| Change      | Beta    | 添加了 [getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)、[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta) 和 [getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta) API。 这些 API 取代了 SfbOrganizerActivity API。 |
| Change      | Beta    | 添加了 [getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)、[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta) 和 [getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta) API。 这些 API 取代了 SfbParticipantActivity API。 |
| Change      | Beta    | 添加了 [getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)、[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta) 和 [getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta) API。 这些 API 取代了 SfbP2PActivity API。 |
| Change      | Beta    | 添加了 [getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta)、[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta) 和 [getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta) API。 这些 API 取代了 YammerActivity API。 |
| Change      | Beta    | 添加了 [getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta)、[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta) 和 [getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta) API。 这些 API 取代了 YammerDeviceUsage API。 |
| 更改      | Beta    | 添加了 [getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta)、[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta) 和 [getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta) API。 这些 API 取代了 YammerGroupsActivity API。 |

### <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|添加了新的 [team](/graph/api/resources/team?view=graph-rest-beta) 实体。|
|添加项|Beta|添加了对 [team](/graph/api/resources/team?view=graph-rest-beta) 实体执行的 [create](/graph/api/team-put-teams?view=graph-rest-beta)、[get](/graph/api/team-get?view=graph-rest-beta) 和 [update](/graph/api/team-update?view=graph-rest-beta) 操作。|

### <a name="users--outlook-settings"></a>用户|Outlook 设置

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
|添加项 | Beta | 向 [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) 添加了新的 **workingHours** 属性。 请参阅 [workingHours 资源类型](/graph/api/resources/workinghours?view=graph-rest-beta)，获取有关受支持用例的信息。|
|添加项 | beta | 添加了以下新复杂类型： <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-beta) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-beta) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-beta) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-beta) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-beta)|


## <a name="september-2017"></a>2017 年 9 月

### <a name="calendar-outlook"></a>日历 (Outlook)

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | Beta          | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 实体添加了 [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) 和 [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) 函数。 |
| 添加项        | Beta          | 向 [event](/graph/api/resources/event?view=graph-rest-beta) 实体添加了 **locations** 属性，以支持组织与会者可以从多个位置参加的事件。 |
| 添加项        | Beta          | 向 [location](/graph/api/resources/location?view=graph-rest-beta) 复杂类型添加了 **locationType** 属性。 |
| 添加项        | Beta          | 向 [location](/graph/api/resources/location?view=graph-rest-beta) 复杂类型添加了 **uniqueId** 和 **uniqueIdType** 属性。 在这种情况下，这些属性仅供内部使用。 |
| 更改          | v1.0 和 Beta | 在用户已与登录用户共享日历，或已将其邮箱委派给登录用户时，此行为增强功能可获取该共享日历或其事件内容。 在这种情况下，只要登录 用户已经向应用提供了委派权限，应用即可指定该用户的 ID 或用户主体名称来[获取该共享日历](/graph/api/calendar-get?view=graph-rest-1.0)，或者[获取该共享日历中的事件](/graph/api/user-list-events?view=graph-rest-1.0)。 |

### <a name="devices-and-apps-microsoft-intune"></a>设备和应用 (Microsoft Intune)

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加项    | Beta    | 添加了新实体：<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[azureADWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta)<br/>[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)<br/>[windows10NetworkBoundaryConfiguration](/graph/api/resources/intune-deviceconfig-windows10networkboundaryconfiguration?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 新增了复杂类型：<br/>[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-beta)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-beta)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-beta)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-beta)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-beta)<br/>[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-beta)<br/>windowsNetworkIsolationCloudResource<br/>windowsNetworkIsolationCloudResourceCollection<br/>windowsNetworkIsolationIPRangeCollection<br/>[windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta)<br/>windowsNetworkIsolationResourceCollection<br/> |
| 添加项    | Beta    | 在 [windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta) 上添加了 [sync](/graph/api/intune-enrollment-windowsautopilotsettings-sync?view=graph-rest-beta) 操作 |
| Addition    | Beta    | 在 [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-enrollment-windowsautopilotdeploymentprofile-assign?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 上添加了 localActions 操作 |
| 添加项    | Beta    | 在 [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) 上添加了 [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 集合上添加了 uploadDepToken 操作 |
| 添加项    | Beta    | 在 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 集合上添加了 syncWithAppleDeviceEnrollmentProgram 操作 |
| 添加项    | Beta    | 在 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 上添加了 updateMobileAppIdentifierDeployments 操作 |
| 添加项    | Beta    | 在 [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) 上添加了 assign 操作 |
| 添加项    | Beta    | 在 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 上添加了 assign 操作 |
| 添加项    | Beta    | 在 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 上添加了 assign 操作 |
| 添加项    | Beta    | 在 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 集合上添加了 getEncryptionPublicKey 函数 |
| 更改      | Beta    | 向 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体添加了 **requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity** 和 **conditionStatementId** 属性 |
| 更改      | Beta    | 向 [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) 实体添加了 **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders** 和 **requireCompanyPortalAppIntegrity** 属性 |
| 更改      | Beta    | 向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **blockCrossProfileCopyPaste** 和 **requireAppVerify** 属性 |
| 更改      | Beta    | 向 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **kioskModeApps** 和 **requireAppVerify** 属性 |
| 更改      | Beta    | 从 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **kioskModeManagedApps** 属性 |
| 更改      | Beta    | 从 cloudPkiSubscription 实体中删除了 **cloudPkiProvider**、**createdDateTime**、**description**、**lastModifiedDateTime**、**displayName**、**syncStatus**、**lastSyncError**、**lastSyncDateTime**、**credentials**、**trustedRootCertificate** 和 **version** 属性 |
| 更改      | Beta    | 从 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 实体中删除了 **assignmentStatus**、**assignmentProgress** 和 **assignmentErrorMessage** 属性 |
| 更改      | Beta    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **adminConsent** 属性 |
| 更改      | Beta    | 向 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 实体添加了 **vppTokenOrganizationName**、**vppTokenAccountType** 和 **vppTokenAppleId** 属性 |
| 更改      | Beta    | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **deviceEnrollmentType**、**wiFiMacAddress** 和 **deviceHealthAttestationState** 属性 |
| 更改      | Beta    | 向 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 实体添加了 **legacyAppConfiguration** 属性 |
| 更改      | Beta    | 向 [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta) 实体添加了 **notApplicableCount** 属性 |
| 更改      | Beta    | 向 [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta) 实体添加了 **notApplicableCount** 属性 |
| 更改      | Beta    | 向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **firewallBlockStatefulFTP**、**firewallIdleTimeoutForSecurityAssociationInSeconds**、**firewallPreSharedKeyEncodingMethod**、**firewallIPSecExemptionsAllowNeighborDiscovery**、**firewallIPSecExemptionsAllowICMP**、**firewallIPSecExemptionsAllowRouterDiscovery**、**firewallIPSecExemptionsAllowDHCP**、**firewallCertificateRevocationListCheckMethod**、**firewallMergeKeyingModuleSettings**、**firewallPacketQueueingMethod**、**firewallProfileDomain**、**firewallProfilePublic**、**firewallProfilePrivate**、**defenderAttackSurfaceReductionExcludedPaths**、**defenderOfficeAppsOtherProcessInjectionType**、**defenderOfficeAppsExecutableContentCreationOrLaunchType**、**defenderOfficeAppsLaunchChildProcessType**、**defenderOfficeMacroCodeAllowWin32ImportsType**、**defenderScriptObfuscatedMacroCodeType**、**defenderScriptDownloadedPayloadExecutionType**、**defenderEmailContentExecutionType**、**defenderGuardMyFoldersType**、**defenderGuardedFoldersAllowedAppPaths**、**defenderAdditionalGuardedFolders**、**defenderNetworkProtectionType**、**defenderExploitProtectionXml**、**defenderExploitProtectionXmlFileName**、**defenderSecurityCenterBlockExploitProtectionOverride**、**appLockerApplicationControl**、**applicationGuardBlockClipboardSharing**、**applicationGuardAllowPrintToPDF**、**applicationGuardAllowPrintToXPS**、**applicationGuardAllowPrintToLocalPrinters**、**applicationGuardAllowPrintToNetworkPrinters** 和 **bitLockerDisableWarningForOtherDiskEncryption** 属性 |
| 更改      | Beta    | 向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **displayAppListWithGdiDPIScalingTurnedOn**、**displayAppListWithGdiDPIScalingTurnedOff**、**messagingBlockSync**、**messagingBlockMMS** 和 **messagingBlockRichCommunicationServices** 属性 |
| 更改      | Beta    | 从 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体中删除了 **bluetoothDeviceName** 属性 |
| 更改      | Beta    | 从 [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) 实体中删除了 **deviceAccountBlockExchangeServices**、**deviceAccountEmailAddress**、**deviceAccountExchangeServerAddress**、**deviceAccountRequirePasswordRotation** 和 **deviceAccountSessionInitiationProtocolAddress** 属性 |
| 更改      | Beta    | 向 [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) 实体添加了 **localActions** 导航属性 |
| 更改      | Beta    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **windowsAutopilotSettings**、**windowsAutopilotDeviceIdentities**、**windowsAutopilotDeploymentProfiles**、**deviceEnrollmentConfigurations**、**deviceManagementPartners** 和 **depOnboardingSettings** 导航属性 |
| 更改      | Beta    | 从 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体中删除了 **cloudPkiSubscriptions** 导航属性 |
| 更改      | Beta    | 向 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体添加了 **assignments** 导航属性 |
| 更改      | Beta    | 向 [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) 实体添加了 **assignments** 导航属性 |
| 更改      | Beta    | 向 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 实体添加了 **assignments** 导航属性 |

### <a name="files-onedrive-for-business"></a>文件 (OneDrive for Business)

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 向 [Drive][] 资源添加了 **system** 属性。 |
| 添加项        | v1.0        | 向 [Drive][] 资源添加了 **list** 关系。 |
| 添加项        | v1.0        | 向 [DriveItem][] 资源添加了 **listItem** 关系。 |
| 添加项        | v1.0        | 向 [SharedDriveItem][] 资源添加了 **list** 和 **listItem** 关系。 |
| 添加项        | v1.0        | 新增了复杂类型：[FolderView][]  |
| 添加项        | v1.0        | 向 [Folder][] 复杂类型添加了 **view** 属性。 |
| 添加项        | v1.0        | 向 [ItemReference][] 复杂类型添加了 **driveType** 属性 |
| 添加项        | v1.0        | 向 [Video][] 复杂类型添加了 **audioBitsPerSample**、**audioChannels**、**audioFormat**、**audioSamplesPerSecond**、**fourCC** 和 **frameRate** 属性。 |
| 添加项        | beta        | 向 [Drive][Drive-beta] 资源添加了 **system** 属性。 |
| 添加项        | beta        | 向 [Drive][Drive-beta] 资源添加了 **activities** 关系。 |
| 添加项        | beta        | 向 [DriveItem][DriveItem-beta] 资源添加了 **publication** 属性。 |
| 添加项        | beta        | 向 [DriveItem][DriveItem-beta] 资源添加了 **activities** 和 **versions** 关系。 |
| 添加项        | beta        | 添加了新实体：[DriveItemVersion][DriveItemVersion-beta]、[ItemActivity][ItemActivity-beta]。 |
| 添加项        | beta        | 新增了复杂类型：[CommentAction][CommentAction-beta]、[CreateAction][CreateAction-beta]、[DeleteAction][DeleteAction-beta]、[EditAction][EditAction-beta]、[ItemActionSet][ItemActionSet-beta]、[ItemActivityTimeSet][ItemActivityTimeSet-beta]、[MentionAction][MentionAction-beta]、[MoveAction][MoveAction-beta]、[PublicationFacet][PublicationFacet-beta]、[RenameAction][RenameAction-beta]、[RestoreAction][RestoreAction-beta]、[ShareAction][ShareAction-beta] 和 [VersionAction][VersionAction-beta]。 |
| 添加项        | beta        | 向 [ItemReference][ItemReference-beta] 复杂类型添加了 **driveType** 属性。 |
| 删除        | beta        | 从 [SharepointIds][SharepointIds-beta] 复杂类型中删除了 **tenantId** 属性。 |
| 添加项        | v1.0        | 向 [Video][Video-beta] 复杂类型添加了 **audioBitsPerSample**、**audioChannels**、**audioFormat**、**audioSamplesPerSecond**、**fourCC** 和 **frameRate** 属性。 |
| 添加项        | beta        | 在 [DriveItem][CheckIn-beta] 资源上添加了 [CheckIn][CheckOut-beta] 和 [CheckOut][DriveItem-beta] 操作。 |
| 添加项        | beta        | 在 **DriveItem** 资源上的 **CreateLink** 操作上添加了 **expirationDateTime**、**password**、[message][CreateLink-beta] 和 [recipients][DriveItem-beta] 属性。 |

[Drive]: /graph/api/resources/drive?view=graph-rest-1.0
[DriveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[SharedDriveItem]: /graph/api/resources/shareddriveitem?view=graph-rest-1.0
[FolderView]: /graph/api/resources/folderview?view=graph-rest-1.0
[Folder]: /graph/api/resources/folder?view=graph-rest-1.0
[ItemReference]: /graph/api/resources/itemreference?view=graph-rest-1.0
[Video]: /graph/api/resources/video?view=graph-rest-1.0
[Drive-beta]: /graph/api/resources/drive?view=graph-rest-beta
[DriveItem-beta]: /graph/api/resources/driveitem?view=graph-rest-beta
[DriveItemVersion-beta]: /graph/api/resources/driveitemversion?view=graph-rest-beta
[ItemActivity-beta]: /graph/api/resources/itemactivity?view=graph-rest-beta
[CommentAction-beta]: /graph/api/resources/commentaction?view=graph-rest-beta
[CreateAction-beta]: /graph/api/resources/createaction?view=graph-rest-beta
[DeleteAction-beta]: /graph/api/resources/deleteaction?view=graph-rest-beta
[EditAction-beta]: /graph/api/resources/editaction?view=graph-rest-beta
[ItemActionSet-beta]: /graph/api/resources/itemactionset?view=graph-rest-beta
[ItemActivityTimeSet-beta]: /graph/api/resources/itemactivitytimeset?view=graph-rest-beta
[MentionAction-beta]: /graph/api/resources/mentionaction?view=graph-rest-beta
[MoveAction-beta]: /graph/api/resources/moveaction?view=graph-rest-beta
[PublicationFacet-beta]: /graph/api/resources/publicationfacet?view=graph-rest-beta
[RenameAction-beta]: /graph/api/resources/renameaction?view=graph-rest-beta
[RestoreAction-beta]: /graph/api/resources/restoreaction?view=graph-rest-beta
[ShareAction-beta]: /graph/api/resources/shareaction?view=graph-rest-beta
[VersionAction-beta]: /graph/api/resources/versionaction?view=graph-rest-beta
[ItemReference-beta]: /graph/api/resources/itemreference?view=graph-rest-beta
[SharepointIds-beta]: /graph/api/resources/sharepointids?view=graph-rest-beta
[Video-beta]: /graph/api/resources/video?view=graph-rest-beta
[CheckIn-beta]: /graph/api/driveitem-checkin?view=graph-rest-beta
[CheckOut-beta]: /graph/api/driveitem-checkout?view=graph-rest-beta
[CreateLink-beta]: /graph/api/driveitem-createlink?view=graph-rest-beta

### <a name="mail"></a>邮件 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta 版本        | 向 [message](/graph/api/resources/message?view=graph-rest-beta) 实体添加了 **internetMessageHeaders** 属性。 |
| 添加        | Beta 版本        | 添加了 [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-beta) 复杂类型。 |
| 添加项        | Beta 版本        | 向 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) 实体添加了 **messageRules** 导航属性。 **messageRules** 是 [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) 实例的集合。 |
| 添加        | Beta 版本        | 添加了 [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) 实体，以及 [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-beta)、[messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-beta) 和 [sizeRange](/graph/api/resources/sizerange?view=graph-rest-beta) 复杂类型。 |
| 添加        | Beta        | 添加了消息规则的以下 CRUD 操作：[创建](/graph/api/mailfolder-post-messagerules?view=graph-rest-beta)、[列出](/graph/api/mailfolder-list-messagerules?view=graph-rest-beta)、[获取](/graph/api/messagerule-get?view=graph-rest-beta)、[更新](/graph/api/messagerule-update?view=graph-rest-beta)和[删除](/graph/api/messagerule-delete?view=graph-rest-beta)。 |

### <a name="personal-contacts"></a>个人联系人 

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改          | v1.0 和 beta | 在用户已与登录用户共享联系人文件夹，或已将其邮箱委派给登录用户时，此行为增强功能可获取该共享联系人文件夹或其联系人内容。 在这种情况下，只要登录 用户已经向应用提供了委派权限，应用即可指定该用户的 ID 或用户主体名称来[获取该共享联系人文件夹](/graph/api/contactfolder-get?view=graph-rest-1.0)，或者[获取该共享文件夹中的联系人](/graph/api/user-list-contacts?view=graph-rest-1.0)。 |

### <a name="sites-and-lists"></a>站点和列表 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 添加了新实体：[ColumnDefinition][]、[ColumnLink][]、[ContentType][]、[List][]、[ListItem][] |
| 添加项        | v1.0        | 向 [Site][] 资源添加了 **columns**、**contentTypes**、**items** 和 **lists** 关系。 |
| 添加项        | v1.0        | 新增了复杂类型：[BooleanColumn][]、[CalculatedColumn][]、[ChoiceColumn][]、[ContentTypeInfo][]、[ContentTypeOrder][]、[CurrencyColumn][]、[DateTimeColumn][]、[DefaultColumnValue][]、[ListInfo][]、[LookupColumn][]、[NumberColumn][]、[PersonOrGroupColumn][]、[SystemFacet][]、[TextColumn][]。 |
| 添加项        | beta        | 添加了新实体：[BaseItemVersion][BaseItemVersion-beta]、[ColumnLink][ColumnLink-beta]、[ContentType][ContentType-beta]、[ListItemVersion][ListItemVersion-beta], |
| 添加项        | beta        | 向 [ColumnDefinition][ColumnDefinition-beta] 添加了 **columnGroup**、**currency**、**defaultValue** 和 **displayName** 属性。 |
| 添加项        | beta        | 向 [List][List-beta] 资源添加了**displayName** 和 **system** 属性。 |
| 添加项        | beta        | 向 [List][List-beta] 资源添加了 **activities** 和 **contentTypes** 关系。 |
| 添加项        | beta        | 向 [ListItem][ListItem-beta] 资源添加了 **contentType** 属性。 |
| 添加项        | beta        | 向 [ListItem][ListItem-beta] 资源添加了 **activities** 和 **versions** 关系。 |
| 添加项        | beta        | 向 [Site][Site-beta] 资源添加了 **contentTypes** 关系。 |
| 添加项        | beta        | 向 [BooleanColumn][BooleanColumn-beta] 类型添加了 **outputType** 属性。 |
| 添加项        | beta        | 新增了复杂类型：[ContentTypeInfo][ContentTypeInfo-beta]、[ContentTypeOrder][ContentTypeOrder-beta]、[CurrencyColumn][CurrencyColumn-beta] 和 [SystemFacet][SystemFacet-beta]。 |
| 添加项        | beta        | 向 [ListInfo][ListInfo-beta] 复杂类型添加了 **contentTypesEnabled** 属性。 |
| 添加项        | beta        | 向 [LookupColumn][LookupColumn-beta] 复杂类型添加了 **allowUnlimitedLength** 属性。 |
| 更改          | beta        | 在 [LookupColumn][LookupColumn-beta] 复杂类型上将 **allowMultipleValue** 属性重命名为 **allowMultipleValues**。 |
| 更改          | beta        | 在 [PersonOrGroupColumn][PersonOrGroupColumn-beta] 复杂类型上将 **chooseFrom** 属性重命名为 **chooseFromType**。 |
| 删除        | beta        | 在 [NumberColumn][NumberColumn-beta] 复杂类型上删除了 **locale** 属性。 |
| 删除        | beta        | 从[PersonOrGroupColumn][PersonOrGroupColumn-beta] 复杂类型中删除了 **enforceUniqueValues** 属性。 |
| 添加项        | beta        | 向 [SiteCollection][SiteCollection-beta] 复杂类型添加了 **dataLocationCode** 和 **root** 属性。 |

[BaseItemVersion-beta]: /graph/api/resources/baseitemversion?view=graph-rest-beta
[BooleanColumn-beta]:  /graph/api/resources/booleanColumn?view=graph-rest-beta
[BooleanColumn]: /graph/api/resources/booleancolumn?view=graph-rest-1.0
[CalculatedColumn]: /graph/api/resources/calculatedcolumn?view=graph-rest-1.0
[ChoiceColumn]: /graph/api/resources/choicecolumn?view=graph-rest-1.0
[ColumnDefinition-beta]: /graph/api/resources/columndefinition?view=graph-rest-beta
[ColumnDefinition]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[ColumnLink-beta]: /graph/api/resources/columnlink?view=graph-rest-beta
[ColumnLink]: /graph/api/resources/columnlink?view=graph-rest-1.0
[ContentType-beta]: /graph/api/resources/contenttype?view=graph-rest-beta
[ContentType]: /graph/api/resources/contenttype?view=graph-rest-1.0
[ContentTypeInfo-beta]: /graph/api/resources/contenttypeinfo?view=graph-rest-beta
[ContentTypeInfo]: /graph/api/resources/contenttypeinfo?view=graph-rest-1.0
[ContentTypeOrder-beta]: /graph/api/resources/contenttypeorder?view=graph-rest-beta
[ContentTypeOrder]: /graph/api/resources/contenttypeorder?view=graph-rest-1.0
[CurrencyColumn-beta]: /graph/api/resources/currencycolumn?view=graph-rest-beta
[CurrencyColumn]: /graph/api/resources/currencycolumn?view=graph-rest-1.0
[DateTimeColumn]: /graph/api/resources/datetimecolumn?view=graph-rest-1.0
[DefaultColumnValue]: /graph/api/resources/defaultcolumnvalue?view=graph-rest-1.0
[List-beta]: /graph/api/resources/list?view=graph-rest-beta
[List]: /graph/api/resources/list?view=graph-rest-1.0
[ListInfo-beta]: /graph/api/resources/listinfo?view=graph-rest-beta
[ListInfo]: /graph/api/resources/listinfo?view=graph-rest-1.0
[ListItem-beta]: /graph/api/resources/listitem?view=graph-rest-beta
[ListItem]: /graph/api/resources/listitem?view=graph-rest-1.0
[ListItemVersion-beta]: /graph/api/resources/listitemversion?view=graph-rest-beta
[LookupColumn-beta]: /graph/api/resources/lookupcolumn?view=graph-rest-beta
[LookupColumn]: /graph/api/resources/lookupcolumn?view=graph-rest-1.0
[NumberColumn-beta]: /graph/api/resources/numbercolumn?view=graph-rest-beta
[NumberColumn]: /graph/api/resources/numbercolumn?view=graph-rest-1.0
[PersonOrGroupColumn-beta]: /graph/api/resources/personorgroupcolumn?view=graph-rest-beta
[PersonOrGroupColumn]: /graph/api/resources/personorgroupcolumn?view=graph-rest-1.0
[Site-beta]: /graph/api/resources/site?view=graph-rest-beta
[Site]: /graph/api/resources/site?view=graph-rest-1.0
[SiteCollection-beta]: /graph/api/resources/sitecollection?view=graph-rest-beta
[SystemFacet-beta]: /graph/api/resources/systemfacet?view=graph-rest-beta
[SystemFacet]: /graph/api/resources/systemfacet?view=graph-rest-1.0
[TextColumn]: /graph/api/resources/textcolumn?view=graph-rest-1.0


### <a name="users--outlook-settings"></a>用户|Outlook 设置

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | 向 [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) 实体添加了新的 **masterCategories** 导航属性。 **masterCategories** 是 [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) 对象的集合。 |
| 添加项        | Beta        | 添加了 [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) 实体。 |
| 添加项        | Beta        | 添加了 [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) 的以下 CRUD 操作：[创建](/graph/api/outlookuser-post-mastercategories?view=graph-rest-beta)、[获取](/graph/api/outlookcategory-get?view=graph-rest-beta)、[更新](/graph/api/outlookcategory-update?view=graph-rest-beta)和[删除](/graph/api/outlookcategory-delete?view=graph-rest-beta)。 |
| 添加项        | Beta        | 向 [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) 实体添加了新的 [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-beta) 函数。 |
| 添加项        | Beta        | 向 [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) 实体添加了新的 [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-beta) 函数。 |


## <a name="august-2017"></a>2017 年 8 月

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加项    | Beta    | 添加了新实体：<br/>[windowsPrivacyDataAccessControlItem](/graph/api/resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 新增了复杂类型：<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-beta) 操作 |
| 添加    | Beta    | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-beta) 操作 |
| 添加    | Beta    | 在 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 上添加了 [windowsPrivacyAccessControls](/graph/api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols?view=graph-rest-beta) 操作 |
| Change      | Beta    | 向 [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) 实体添加了 **automaticallyUpdateApps** 和 **countryOrRegion** 属性 |
| Change      | Beta    | 向 [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) 实体添加了 **enableAuthenticationViaCompanyPortal** 属性 |
| Change      | Beta    | 向 [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) 实体添加了 **notificationMessageCCList** 属性 |
| Change      | Beta    | 向 [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) 实体添加了 **notApplicableCount** 属性 |
| Change      | Beta    | 向 [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) 实体添加了 **notApplicableCount** 属性 |
| Change      | Beta    | 向 [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) 实体添加了 **notApplicableCount** 属性 |
| Change      | Beta    | 向 [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) 实体添加了 **notApplicableCount** 属性 |
| Change      | Beta    | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **configurationManagerClientEnabledFeatures** 属性 |
| Change      | Beta    | 从 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 实体中删除了 **intuneBrand** 属性 |
| Change      | Beta    | 向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **smartScreenEnableInShell**、**smartScreenBlockOverrideForFiles**、**applicationGuardEnabled**、**applicationGuardBlockFileTransfer**、**applicationGuardBlockNonEnterpriseContent**、**applicationGuardAllowPersistence** 和 **applicationGuardForceAuditing** 属性 |
| Change      | Beta    | 向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **searchBlockDiacritics**、**searchDisableAutoLanguageDetection**、**searchDisableIndexingEncryptedItems**、**searchEnableRemoteQueries**、**searchDisableUseLocation**、**searchDisableIndexerBackoff**、**searchDisableIndexingRemovableDrive**、**searchEnableAutomaticIndexSizeManangement**、**smartScreenEnableAppInstallControl** 和 **privacyAdvertisingId** 属性 |
| Change      | Beta    | 从 [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) 实体中删除了 **settingsDeviceName** 属性 |
| Change      | Beta    | 从 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体中删除了 **restartMode** 属性 |
| 更改      | Beta    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **detectedApps** 和 **managedDevices** 导航属性 |
| 更改      | Beta    | 向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **privacyAccessControls** 导航属性 |
| Change      | Beta    | 向 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型添加了 **secureByDefault** 属性 |
| Change      | Beta    | 向 [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) 复杂类型添加了 **restartMode** 属性 |

### <a name="groups"></a>组

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加了 [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-beta) 实体。 |
| 添加        | Beta        | 添加了以下组生命周期策略 API：[create](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-beta)、[list](/graph/api/grouplifecyclepolicy-list?view=graph-rest-beta)、[get](/graph/api/grouplifecyclepolicy-get?view=graph-rest-beta)、[update](/graph/api/grouplifecyclepolicy-update?view=graph-rest-beta)、[delete](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-beta)、[add group](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-beta)、[remove group](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-beta) 和 [renew a group](/graph/api/grouplifecyclepolicy-renewgroup?view=graph-rest-beta)。 |
| 添加        | Beta        | 向 [group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了 [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-beta) 函数。 |

### <a name="notes"></a>注释 

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项        | v1.0 和 Beta | 向 **site** 添加了 [onenote](/graph/api/resources/onenote?view=graph-rest-1.0) 导航属性。 |
| 添加项        | Beta          | Added the target *siteCollectionId* and target *siteId* parameters for the copy operations. For example: [CopyNotebook](/graph/api/notebook-copynotebook?view=graph-rest-1.0). |

### <a name="social-and-workplace-intelligence--people"></a>社交和工作场所智能 | 人员

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | Added the [People APIs](/graph/api/resources/person?view=graph-rest-1.0) to v1.0. For details about the People API, see [Get relevant information about people](people-example.md). |
| 新增        | v1.0        | 新增了 People.Read.All 权限。 若要了解详细信息，请参阅[权限](permissions-reference.md)。 |
| 新增        | v1.0        | 新增了 [personType](/graph/api/resources/persontype?view=graph-rest-1.0) 资源。 |
| 更改          | v1.0        | [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) 资源替换了 **rankedEmailAddress** 资源。 |
| 更改          | v1.0        | 更新了 [person](/graph/api/resources/person?view=graph-rest-1.0) 资源，如下所述：<ul><li>**scoredEmailAddresses** 属性（[scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) 类型的集合）替换了 **emailAddresses** 属性</li><li>**jobTitle** 属性替换了 **title** 属性</li><li>删除了 **sources** 和 **mailboxType** 属性</li><li>**personType** 属性现在是 [personType](/graph/api/resources/persontype?view=graph-rest-1.0) 类型（而不是字符串类型），并替换了旧属性 **sources** 和 **mailboxType** 的功能</li><li>添加了 **imAddress** 属性</li></ul> |
| 删除        | v1.0        | 删除了 **personDataSource** 资源。 |

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 添加了 **employeeId** 属性 |

## <a name="july-2017"></a>2017 年 7 月

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| 更改类型 | 版本 | 说明                              |
| :--------------- | :------ | :--------------------------------------- |
| 添加         | Beta    | 在 [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-apps-iosmobileappconfiguration-assign?view=graph-rest-beta) 操作 |
| 添加项         | Beta    | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-beta) 操作 |
| Change           | Beta    | 向 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **appsInstallAllowList**、**appsLaunchBlockList** 和 **appsHideList** 属性 |
| Change           | Beta    | 向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **disableAppEncryptionIfDeviceEncryptionIsEnabled** 属性 |
| Change           | Beta    | 向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **disableAppEncryptionIfDeviceEncryptionIsEnabled** 属性 |
| Change           | Beta    | 向 [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性 |
| Change           | Beta    | 向 [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性 |
| Change           | Beta    | 向 [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性 |
| Change           | Beta    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **subscriptions** 属性 |
| Change           | Beta    | 向 [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) 实体添加了 **version** 属性 |
| Change           | Beta    | 向 [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) 实体添加了 **utcTimeOffsetInMinutes** 属性 |
| Change           | Beta    | 向 [iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性 |
| Change           | Beta    | 向 [macOSWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macoswificonfiguration?view=graph-rest-beta) 实体添加了 **preSharedKey** 属性 |
| Change           | Beta    | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **phoneNumber**、**androidSecurityPatchLevel** 和 **userDisplayName** 属性 |
| Change           | Beta    | 向 [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) 实体添加了 **userName**、**deviceModel**、**platform** 和 **complianceGracePeriodExpirationDateTime** 属性 |
| Change           | Beta    | 向 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) 实体添加了 **userPrincipalName** 属性 |
| Change           | Beta    | 向 [onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta) 实体添加了 **overrideDefaultRule** 属性 |
| Change           | Beta    | 向 [userAppInstallStatus](/graph/api/resources/intune-apps-userappinstallstatus?view=graph-rest-beta) 实体添加了 **userPrincipalName** 属性 |
| Change           | Beta    | 向 [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) 实体添加了 **connectAppBlockAutoLaunch**、**deviceAccountBlockExchangeServices**、**deviceAccountEmailAddress**、**deviceAccountExchangeServerAddress**、**deviceAccountRequirePasswordRotation**、**deviceAccountSessionInitiationProtocolAddress**、**settingsBlockMyMeetingsAndFiles**、**settingsBlockSessionResume**、**settingsBlockSigninSuggestions**、**settingsDefaultVolume**、**settingsScreenTimeoutInMinutes**、**settingsSessionTimeoutInMinutes** 和 **settingsSleepTimeoutInMinutes** 属性 |
| Change           | Beta    | 向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **deploymentSummary** 导航属性 |
| 更改           | Beta    | 向 [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 复杂类型添加了 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性 |
| Change           | Beta    | 将 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性添加到了 [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 复杂类型中 |
| 更改           | Beta    | 向 [deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-beta) 复杂类型添加了 **unknownCount** 属性 |

### <a name="identity-and-access--group-setting"></a>身份和访问|组设置

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 添加了组设置支持。<br/>新资源类型：[groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0)、[groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0)、[settingValue](/graph/api/resources/settingvalue?view=graph-rest-1.0) 和 [settingTemplateValue](/graph/api/resources/settingtemplatevalue?view=graph-rest-1.0) |
| 更改          | v1.0        | 将属性 **classification** 和导航属性**settings** 添加到[组](/graph/api/resources/group?view=graph-rest-1.0) |


## <a name="june-2017"></a>2017 年 6 月

### <a name="calendar"></a>日历

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 将以下 4 个 [calendar](/graph/api/resources/calendar?view=graph-rest-1.0)属性升级到 v1.0：**canEdit**、**canShare**、**canViewPrivateItems** 和 **owner**。 |

### <a name="cross-device-experiences"></a>跨设备体验

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加了以下资源和 API：<br/>[活动](/graph/api/resources/projectrome-activity?view=graph-rest-beta)<br/>[创建或替换活动](/graph/api/projectrome-put-activity?view=graph-rest-beta)<br/>[删除活动](/graph/api/projectrome-delete-activity?view=graph-rest-beta)<br/>[历史记录项](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta)<br/>[创建或替换历史记录项](/graph/api/projectrome-put-historyitem?view=graph-rest-beta)<br/>[删除历史记录项](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加项    | Beta    | 添加的新实体：<br/>[defaultDeviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-defaultdevicecompliancepolicy?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[deviceManagementScriptDeviceState](/graph/api/resources/intune-devicefe-devicemanagementscriptdevicestate?view=graph-rest-beta)<br/>[deviceManagementScriptRunSummary](/graph/api/resources/intune-devicefe-devicemanagementscriptrunsummary?view=graph-rest-beta)<br/>[deviceManagementScriptUserState](/graph/api/resources/intune-devicefe-devicemanagementscriptuserstate?view=graph-rest-beta)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta)<br/>[windowsManagedDevice](/graph/api/resources/intune-devicefe-windowsmanageddevice?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-devicefe-windowsmanagementapphealthstate?view=graph-rest-beta)<br/>[windowsManagementAppHealthSummary](/graph/api/resources/intune-devicefe-windowsmanagementapphealthsummary?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 新增了复杂类型：<br/>[bitLockerFixedDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerfixeddrivepolicy?view=graph-rest-beta)<br/>[bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-beta)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devicefe-deleteuserfromsharedappledeviceactionresult?view=graph-rest-beta)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-beta)<br/> |
| 删除    | Beta    | 删除了以下实体：<br/>**deviceManagementScriptState**<br/> |
| 删除    | Beta    | 在[用户](/graph/api/resources/intune-devicefe-user?view=graph-rest-beta)上删除了 wipeByDeviceTag 操作 |
| 更改      | Beta 版本    | 向 [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **innerAuthenticationProtocolForEapTtls**、**innerAuthenticationProtocolForPeap** 和 **outerIdentityPrivacyTemporaryValue** 属性 |
| 更改      | Beta 版本    | 从 [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) 实体删除了 **nonEapAuthenticationMethodForEapTtls**、**nonEapAuthenticationMethodForPeap** 和 **enableOuterIdentityPrivacy** 属性 |
| 更改      | Beta 版本    | 向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **deployedAppCount** 属性 |
| 更改      | Beta 版本    | 从 [complianceSettingStateSummary](/graph/api/resources/compliancesettingstatesummary?view=graph-rest-beta) 实体删除了 **instanceDisplayName** 和 **settingPlatform** 属性 |
| 更改      | Beta 版本    | 向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **deployedAppCount** 属性 |
| 更改      | Beta 版本    | 向 [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta) 实体添加了 **excludeGroup** 属性 |
| 更改      | Beta 版本    | 从 [deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta) 实体删除了 **instanceDisplayName** 和 **settingPlatform** 属性 |
| 更改      | Beta 版本    | 从 [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) 实体删除了 **devicePlatform** 属性 |
| 更改      | Beta 版本    | 向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 实体添加了 **assignmentStatus**、**assignmentProgress** 和 **assignmentErrorMessage** 属性 |
| 更改      | Beta 版本    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **intuneBrand** 属性 |
| 更改      | Beta    | 向 [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) 实体添加了 **enforceSignatureCheck** 和 **fileName** 属性 |
| 更改      | Beta 版本    | 向 [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **innerAuthenticationProtocolForEapTtls** 和 **outerIdentityPrivacyTemporaryValue** 属性 |
| 更改      | Beta 版本    | 从 [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) 实体删除了 **nonEapAuthenticationMethodForEapTtls** 和 **enableOuterIdentityPrivacy** 属性 |
| 更改      | Beta 版本    | 向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **classroomAppForceUnpromptedScreenObservation**、**keyboardBlockDictation**、**networkUsageRules** 和 **wiFiConnectOnlyToConfiguredNetworks** 属性 |
| 更改      | Beta    | 向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **deployedAppCount** 属性 |
| 更改      | Beta 版本    | 向 [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta) 实体添加了 **preSharedKey** 属性 |
| 更改      | Beta 版本    | 向 [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) 实体添加了 **innerAuthenticationProtocolForEapTtls** 和 **outerIdentityPrivacyTemporaryValue** 属性 |
| 更改      | Beta 版本    | 从 [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) 实体删除了 **nonEapAuthenticationMethodForEapTtls** 和 **enableOuterIdentityPrivacy** 属性 |
| 更改      | Beta 版本    | 从 [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) 实体删除了 **lastModifiedTime** 和 **deployedAppCount** 属性 |
| 更改      | Beta 版本    | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **serialNumber** 属性 |
| 更改      | Beta 版本    | 从 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体删除了 **managementAgents** 属性 |
| 更改      | Beta 版本    | 向 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体添加了 **deployedAppCount** 属性 |
| 更改      | Beta 版本    | 向 [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) 实体添加了 **bitLockerFixedDrivePolicy** 和 **bitLockerRemovableDrivePolicy** 属性 |
| 更改      | Beta 版本    | 向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **enterpriseCloudPrintDiscoveryEndPoint**、**enterpriseCloudPrintOAuthAuthority**、**enterpriseCloudPrintOAuthClientIdentifier**、**enterpriseCloudPrintResourceIdentifier**、**enterpriseCloudPrintDiscoveryMaxLimit**、**enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**、**edgeBlockAddressBarDropdown**、**edgeBlockCompatibilityList**、**edgeClearBrowsingDataOnExit**、**edgeAllowStartPagesModification**、**edgeDisableFirstRunPage**、**edgeBlockLiveTileDataCollection** 和 **edgeSyncFavoritesWithInternetExplorer** 属性 |
| 更改      | Beta    | 向 [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) 实体添加了 **availableVersion** 属性 |
| 更改      | Beta 版本    | 从 [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) 实体删除了 **onboardingStatus**、**deployedVersion** 和 **lastModifiedTime** 属性 |
| 更改      | Beta 版本    | 向 [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta) 实体添加了 **packageIdentityName** 属性 |
| 更改      | Beta 版本    | 向 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 实体添加了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性 |
| 更改      | Beta 版本    | 向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **mobileAppIdentifierDeployments** 导航属性 |
| 更改      | Beta    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceConfigurationUserStateSummaries** 和 **iosUpdateStatuses** 导航属性 |
| 更改      | Beta 版本    | 从 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体删除了 **complianceSettingStateSummaries** 导航属性 |
| 更改      | Beta 版本    | 向 [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) 实体添加了 **runSummary**、**deviceRunStates** 和 **userRunStates** 导航属性 |
| 更改      | Beta 版本    | 从 [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) 实体删除了 **runStates** 导航属性 |
| 更改      | Beta 版本    | 向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性 |
| 更改      | Beta 版本    | 从 [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) 实体删除了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性 |
| 更改      | Beta 版本    | 向 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体添加了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性 |
| 更改      | Beta 版本    | 向 [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) 实体添加了 **healthSummary** 和 **healthStates** 导航属性 |
| 更改      | Beta 版本    | 向 [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) 复杂类型添加了 **applicationId**、**appName**、**platformId**、**userFailures** 和 **deviceFailures** 属性 |
| 更改      | Beta 版本    | 向 [bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy) 复杂类型添加了 **encryptionMethod**、**startupAuthenticationRequired**、**startupAuthenticationBlockWithoutTpmChip**、**startupAuthenticationTpmUsage**、**startupAuthenticationTpmPinUsage**、**startupAuthenticationTpmKeyUsage**、**startupAuthenticationTpmPinAndKeyUsage**、**recoveryOptions** 和 **prebootRecoveryEnableMessageAndUrl** 属性 |
| 更改      | Beta 版本    | 从 [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 复杂类型删除了 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性 |
| 更改      | Beta 版本    | 从 [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 复杂类型删除了 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性 |
| 更改      | Beta 版本    | 向 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型添加了 **windowsCommercialId** 和 **windowsCommercialIdLastModifiedTime** 属性 |
| 更改      | Beta 版本    | 向 [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta) 复杂类型添加了 **address** 属性 |


## <a name="may-2017"></a>2017 年 5 月

### <a name="identity-and-access--application"></a>身份和访问|应用程序

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta 版本        | Application API update. This is first set of changes including property renaming and restructuring of the [application](/graph/api/resources/application?view=graph-rest-beta) entity.<br/>**新实体：**[api](/graph/api/resources/api?view=graph-rest-beta])、[informationalUrl](/graph/api/resources/informationalurl?view=graph-rest-beta)、[installedClient](/graph/api/resources/installedclient?view=graph-rest-beta)、[permissionScope](/graph/api/resources/permissionscope?view=graph-rest-beta)、[preauthorizedApplication](/graph/api/resources/preauthorizedapplication?view=graph-rest-beta)、[Web](/graph/api/resources/web?view=graph-rest-beta)。<br/>**删除的属性：** addIns、appRoles、availableToOtherOrganizations、knownClientApplications、oauth2AllowUrlPathMatching、recordConsentConditions。<br/>**重命名的属性：** appId 重命名为 id，identifierUris 重命名为 applicationAliases，availableToOtherTenants 重命名为 orgRestrictions，mainLogo 重命名为 logo，oauth2Permissions 重命名为 publishedPermissionsScopes，publicClient 重命名为 allowPublicClient，replyUrls 重命名为 redirectUrls。<br/>**新属性：** tags。 |

### <a name="tasks-and-plans"></a>任务和计划
| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 删除        | Beta        | 删除了以下实体：<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="cross-device-experiences"></a>跨设备体验

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加了对 Project Rome 的支持，包括[获取设备列表](/graph/api/user-list-devices?view=graph-rest-beta)、[发送命令到设备](/graph/api/send-device-command?view=graph-rest-beta)和[查看命令状态](/graph/api/get-device-command-status?view=graph-rest-beta)。 |
| 添加项        | Beta        | 增加了对用户[活动](/graph/api/resources/projectrome-activity?view=graph-rest-beta)和 [historyItems](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) 的支持，其中包括 [upsert 活动](/graph/api/projectrome-put-activity?view=graph-rest-beta)和 [upsert historyItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta)。 |

### <a name="identity-and-access--administrative-unit"></a>身份和访问|管理单元

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta        | 已将 [scopedRoleMembership](/graph/api/resources/scopedrolemembership?view=graph-rest-beta) 实体的 roleMemberInfo 属性类型更改为 [identity](/graph/api/resources/identity?view=graph-rest-1.0) |
| 更改          | Beta        | 已将 [user](/graph/api/resources/user?view=graph-rest-beta) 实体的导航属性 scopedAdministratorOf 更改为 scopedRoleMemberOf |
| 更改          | Beta        | 已将 [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) 实体的导航属性 scopedAdministrators 更改为 scopedRoleMembers |
| 更改          | Beta        | 已将 [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta) 实体的导航属性 scopedAdministrators 更改为 scopedMembers |

### <a name="change-notifications"></a>更改通知

|**更改类型**|**Version**|**说明**|
|:--------------|:-----------|:--------------|
| 更改        | Beta       | 添加了用户和组的 [Webhooks](/graph/api/resources/webhooks?view=graph-rest-beta) 支持

### <a name="change-tracking"></a>更改跟踪

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 向 v1.0 添加 delta 函数支持。 向以下实体添加执行 [delta 查询](delta-query-overview.md)功能：<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>有关示例，请参阅以下文章：<br/>[获取组的增量更改](delta-query-groups.md)<br/>[获取文件夹中邮件的增量更改](delta-query-messages.md)<br/>[获取用户的增量更改](delta-query-users.md) |
| 更改          | Beta        | 将其他可选查询筛选功能（按 id）添加到 [users](/graph/api/user-delta?view=graph-rest-beta) 和 [groups](/graph/api/group-delta?view=graph-rest-beta)。 |

### <a name="added-user-resource-support-for-deleted-items"></a>添加了对已删除项目的用户资源支持

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加了对[还原并永久删除用户](/graph/api/resources/directory?view=graph-rest-beta)的支持。 |

### <a name="added-onpremisesprovisioningerror"></a>添加了 OnPremisesProvisioningError

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | beta        | 新实体：[OnPremisesProvisioningError](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-beta) |
| 更改          | beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta)、[group](/graph/api/resources/group?view=graph-rest-beta) 和 [orgcontact](/graph/api/resources/orgcontact?view=graph-rest-beta) 添加了 OnPremisesProvisioningError 属性。 |

### <a name="added-deleteddatetime-property"></a>添加了 deletedDateTime 属性

|**更改类型**|**Version**|**说明**|
|:-------------|:-----------|:--------------|
|更改|beta|向 [user](/graph/api/resources/user?view=graph-rest-beta) 实体添加了 deletedDateTime 属性。
|更改|beta|向 [group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了 deletedDateTime 属性。
|更改|beta|向 [application](/graph/api/resources/application?view=graph-rest-beta) 实体添加了 deletedDateTime 属性。

### <a name="added-domain-operations-to-v10"></a>向 v1.0 添加了域操作

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 向 [domains](/graph/api/resources/domain?view=graph-rest-1.0) 添加了操作。<br/>新实体：</br>[domain](/graph/api/resources/domain?view=graph-rest-1.0)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-1.0)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-1.0)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-1.0)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-1.0)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-1.0)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-1.0)<br/>新操作：</br>[verify](/graph/api/domain-verify?view=graph-rest-1.0) |

### <a name="added-contracts-to-v10"></a>向 v1.0 添加了合同

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 新实体：</br>[contract](/graph/api/resources/contract?view=graph-rest-1.0) |

### <a name="added-licensedetails-to-v10"></a>向 v1.0 添加了 licenseDetails

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 新实体：</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-1.0) |
| 更改          | v1.0        | 针对[用户](/graph/api/resources/user?view=graph-rest-1.0)的新 [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-1.0) 导航属性 |


### <a name="files"></a>文件

|**更改类型**|**Version**|**说明**|
|:--------------|:----------|:--------------|
| 添加 | v1.0 | 添加了 **baseItem** 资源类型，其中包含 **driveItem** 中的基本属性。
| 添加项 | v1.0 和 Beta | 向 **thumbnail** 添加了 **sourceItemId** 属性。 <br/> 向 **sharepointIds** 添加了 **siteUrl** 属性。 <br/> 向 **shared** 添加了 **sharedBy** 和 **sharedDateTime** 属性。 <br/> 向 **remoteItem** 添加了 **shared** 属性。 <br/> 向 **drive** 和 **itemReference** 添加了 **sharepointIds** 属性。 <br/> 向 **fileSystemInfo** 添加了 **lastAccessedDateTime**。 <br/> 向 **sharedDriveItem** 添加了 **driveItem** 和 **site** 导航属性。 <br/> 向 **baseItem** 添加了 **parentReference** 属性。
| 更改 | v1.0 和 Beta | 已将 **driveItem** 和 **sharedDriveItem** 更改为从 **baseItem** 继承。 <br/> 已将 **identity** 标记为“开放类型”。
| Change | Beta | 向 **sharingLink** 添加了 **configuratorUrl** 和 **WebHtml** 属性。 <br/> 向 **folder** 资源类型添加了 **folderView** 资源类型和 **view** 属性。 <br/> 向 **driveItem** 添加了 **listItem** 导航属性。 <br/> 向 **drive** 添加了 **list** 导航属性。


### <a name="open-extensions"></a>开放扩展

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0          | 支持下列资源中的 [openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0)：[device](/graph/api/resources/device?view=graph-rest-1.0)、[group](/graph/api/resources/group?view=graph-rest-1.0)、[organization](/graph/api/resources/organization?view=graph-rest-1.0)、[user](/graph/api/resources/user?view=graph-rest-1.0)。 |
| 添加项        | v1.0 和 beta | When the user is signed-in with a personal Microsoft account, support for open extensions in the following resources - event, post, group, message, contact, and user. (This is in addition to these resources, plus device, group, organization and user, supporting open extensions when the user signs in using a work or school account.) |
| 添加项        | v1.0 和 beta | 支持 `$expand` 在下列资源中[获取开放扩展](/graph/api/opentypeextension-get?view=graph-rest-1.0)：[device](/graph/api/resources/device?view=graph-rest-1.0)、[group](/graph/api/resources/group?view=graph-rest-1.0)、[organization](/graph/api/resources/organization?view=graph-rest-1.0)、[post](/graph/api/resources/post?view=graph-rest-1.0)、[user](/graph/api/resources/user?view=graph-rest-1.0)。 |
| 添加项        | Beta          | 支持 `$expand` 在 [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) 中[获取开放扩展](/graph/api/opentypeextension-get?view=graph-rest-1.0)。 |


### <a name="schema-extensions"></a>架构扩展

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0          | New resource [schemaExtension](/graph/api/resources/schemaextension?view=graph-rest-1.0) and CRUD methods to manage extension definitions for the following resources: [contact](/graph/api/resources/contact?view=graph-rest-1.0), [device](/graph/api/resources/device?view=graph-rest-1.0), [event](/graph/api/resources/event?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0), [user](/graph/api/resources/user?view=graph-rest-1.0). Note that support for [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) is still limited to the beta version as before. |
| 新增        | v1.0          | 下列资源中的现有 POST、GET 和 PATCH方法 - [contact](/graph/api/resources/contact?view=graph-rest-1.0)、[device](/graph/api/resources/device?view=graph-rest-1.0)、[event](/graph/api/resources/event?view=graph-rest-1.0)、[group](/graph/api/resources/group?view=graph-rest-1.0)、[message](/graph/api/resources/message?view=graph-rest-1.0)、[organization](/graph/api/resources/organization?view=graph-rest-1.0)、[post](/graph/api/resources/post?view=graph-rest-1.0)、[user](/graph/api/resources/user?view=graph-rest-1.0) - 现在支持添加、获取、更新或删除作为架构扩展存储在相应资源实例中的自定义数据。 |
| Addition        | v1.0 和 beta | You can now use `$filter` to look for resource instances with properties that match specific extension property values, such as extension name. See this [example](extensibility-schema-groups.md#5-get-a-group-and-its-extension-data) for details. |
| 更改          | v1.0 和 Beta | [删除架构扩展定义](/graph/api/schemaextension-delete?view=graph-rest-1.0)不再会影响访问基于此定义添加的自定义数据。 |
| 更改          | v1.0 和 Beta | 现在可以将架构扩展复杂类型设为 null，以便将架构扩展从资源实例中删除。 |


### <a name="groups"></a>组

|**更改类型**|**Version**|**说明**|
|:--------------|:----------|:--------------|
| 添加 | v1.0 和 beta | 向 **group** 添加了 **drives** 和 **sites** 导航属性。

### <a name="social-and-workplace-intelligence--insights"></a>社交和工作场所智能|见解

|**更改类型**|**Version**|**说明**|
|:-------------|:-----------|:--------------|
|添加|Beta|添加了 [Shared API](/graph/api/resources/insights-shared?view=graph-rest-beta)。<br />新资源：<br />[sharingDetail](/graph/api/resources/insights-sharingdetail?view=graph-rest-beta) <br />[insightIdentity](/graph/api/resources/insights-insightidentity?view=graph-rest-beta) <br />
|添加项|Beta|添加了 [Used API](/graph/api/resources/insights-used?view=graph-rest-beta)。<br />新资源：<br />[usageDetails](/graph/api/resources/insights-usagedetails?view=graph-rest-beta) <br />
|更改|Beta 版本|以下资源中的新 **Type** 属性：<br />[resourceVisualization](/graph/api/resources/insights-resourcevisualization?view=graph-rest-beta)。 <br />
|删除|Beta|删除了以下实体：<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加    | Beta    | 添加的新实体：<br/>[androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta)<br/>[cartToClassAssociation](/graph/api/resources/intune-deviceconfig-carttoclassassociation?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-beta)<br/>[eBookVppGroupAssignment](/graph/api/resources/intune-books-ebookvppgroupassignment?view=graph-rest-beta)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)<br/>[windowsDeviceMalwareState](/graph/api/resources/intune-endpointprotection-windowsdevicemalwarestate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-beta)<br/>[windowsMalwareInformation](/graph/api/resources/intune-endpointprotection-windowsmalwareinformation?view=graph-rest-beta)<br/>[windowsProtectionState](/graph/api/resources/intune-endpointprotection-windowsprotectionstate?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 添加的新复杂类型：<br/>[androidPermissionAction](/graph/api/resources/intune-apps-androidpermissionaction?view=graph-rest-beta)<br/>[bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-beta)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 在 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) 上添加了 [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) 上添加了 [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-beta) 操作 |
| 删除    | Beta    | 删除了以下实体：<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| 删除    | Beta    | 删除了以下复杂类型：<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| 更改      | Beta 版本    | 向 [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **workProfilePasswordBlockFingerprintUnlock**、**workProfilePasswordBlockTrustAgents**、**workProfilePasswordExpirationDays**、**workProfilePasswordMinimumLength**、**workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**、**workProfilePasswordPreviousPasswordBlockCount**、**workProfilePasswordSignInFailureCountBeforeFactoryReset**、**workProfilePasswordRequiredType** 和 **workProfileRequirePassword** 属性 |
| 更改      | Beta 版本    | 向 [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta 版本    | 向 [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta 版本    | 向 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **kioskModeManagedApps** 属性 |
| 更改      | Beta    | 从 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体删除了 **kioskModeManagedAppId** 属性 |
| 更改      | Beta 版本    | 向 [androidPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidpkcscertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta 版本    | 向 [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta 版本    | 从 [calendar](/graph/api/resources/calendar?view=graph-rest-beta) 实体删除了 **hexColor** 属性 |
| 更改      | Beta 版本    | 将 **setting** 和 **platformType** 属性添加到了 [complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta) 实体中 |
| 更改      | Beta 版本    | 从 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体删除了 **windowsManagementAppEnabled** 属性 |
| 更改      | Beta 版本    | 向 [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) 实体添加了 **userName**、**deviceModel** 和 **platform** 属性 |
| 更改      | Beta    | 向 [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) 实体添加了 **userPrincipalName** 和 **deviceModel** 属性 |
| 更改      | Beta    | 将 **platformType**、**setting**、**userId** 和 **userEmail** 属性添加到了 [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) 实体中 |
| 更改      | Beta    | 将 **inGracePeriodCount** 属性添加到了 [deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta) 实体中 |
| 更改      | Beta    | 向 [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) 实体添加了 **userName**、**deviceModel** 和 **platform** 属性 |
| 更改      | Beta    | 从 [event](/graph/api/resources/event?view=graph-rest-beta) 实体删除了 **creationOptions** 属性 |
| 更改      | Beta    | 从 [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta) 实体删除了 **isDelegated** 属性 |
| 更改      | Beta    | 从 [group](/graph/api/resources/group?view=graph-rest-beta) 实体删除了 **unseenConversationsCount** 和 **unseenMessagesCount** 属性 |
| 更改      | Beta    | 向 [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) 实体添加了 **settingXml** 和 **settings** 属性 |
| 更改      | Beta    | 向 [iosPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-iospkcscertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta    | 向 [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta    | 向 [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) 实体添加了 **systemIntegrityProtectionEnabled** 属性 |
| 更改      | Beta    | 向 [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta    | Added the **complianceGracePeriodExpirationDateTime**, **userPrincipalName**. and **imei** properties to the [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) entity |
| 更改      | Beta    | 从 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 实体删除了 **settingXml** 和 **settings** 属性 |
| 更改      | Beta    | 向 [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) 实体添加了 **useSharedComputerActivation**、**updateChannel**、**officePlatformArchitecture** 和 **localesToInstall** 属性 |
| 更改      | Beta    | 从 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 实体删除了 **applePushNotificationCertificateSetting** 属性 |
| 更改      | Beta    | 更改了 [post](/graph/api/resources/post?view=graph-rest-beta) 实体上的以下属性：<br/>将 **sender** 从可选更改为必需<br/> |
| 更改      | Beta    | 向 [softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta) 实体添加了 **compliantUserCount**、**nonCompliantUserCount**、**remediatedUserCount**、**errorUserCount**、**unknownUserCount**、**conflictUserCount**和 **notApplicableUserCount** 属性 |
| 更改      | Beta    | 向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **bluetoothAllowedServices**、**bluetoothBlockPrePairing**、**cellularData**、**defenderDetectedMalwareActions**、**defenderPotentiallyUnwantedAppAction**、**lockScreenAllowTimeoutConfiguration**、**lockScreenBlockCortana**、**lockScreenBlockToastNotifications**、**lockScreenTimeoutInSeconds**、**passwordBlockSimple**、**privacyAutoAcceptPairingAndConsentPrompts**、**privacyBlockInputPersonalization**、**startMenuHideChangeAccountSettings**、**startMenuHideHibernate**、**startMenuHideLock**、**startMenuHideShutDown**、**startMenuHideSignOut**、**startMenuHideSleep**、**startMenuHideSwitchAccount**、**settingsBlockAppsPage**、**settingsBlockGamingPage**、**windowsSpotlightBlockConsumerSpecificFeatures**、**windowsSpotlightBlocked**、**windowsSpotlightBlockOnActionCenter**、**windowsSpotlightBlockTailoredExperiences**、**windowsSpotlightBlockThirdPartyNotifications**、**windowsSpotlightBlockWelcomeExperience**、**windowsSpotlightBlockWindowsTips**、**windowsSpotlightConfigureOnLockScreen** 和 **connectedDevicesServiceBlocked** 属性。 |
| 更改      | Beta    | 从 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体删除了 **automaticUpdateMode**、**automaticUpdateSchedule**、**automaticUpdateTime**、**prereleaseFeatures**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips** 和 **experienceBlockConsumerSpecificFeatures** 属性。 |
| 更改      | Beta    | 向 [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) 实体添加了 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta    | 向 [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta    | 向 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 实体添加了 **indexingEncryptedStoresOrItemsBlocked** 和 **smbAutoEncryptedFileExtensions** 属性 |
| 更改      | Beta    | 更改了 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 实体上的以下属性：<br/>将 **rightsManagementServicesTemplateId** 从必需更改为可选<br/> |
| 更改      | Beta    | 更改了 [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) 实体上的以下属性：<br/>将 **productCode** 从必需更改为可选<br/> |
| 更改      | Beta    | 向 [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性 |
| 更改      | Beta    | 向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **mobileAppConfigurations** 导航属性 |
| 更改      | Beta    | 将 **cartToClassAssociations**、**deviceCompliancePolicySettingStateSummaries**、**remoteAssistancePartners**、**windowsInformationProtectionAppLearningSummaries** 和**windowsMalwareInformation** 导航属性添加到了 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体中 |
| 更改      | Beta    | 向 [eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta) 实体添加了 **eBook** 导航属性 |
| 更改      | Beta    | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **windowsProtectionState** 导航属性 |
| 更改      | Beta    | 向 [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) 实体添加了 **installSummary** 导航属性 |
| 更改      | Beta    | 从 [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) 实体删除了 **outlook** 导航属性 |
| 更改      | Beta    | 从 [windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta) 实体删除了 **healthStates** 导航属性 |
| 更改      | Beta    | 向 [defaultDeviceEnrollmentRestrictions](/graph/api/resources/intune-onboarding-defaultdeviceenrollmentrestrictions?view=graph-rest-beta) 复杂类型添加了 **androidForWorkRestrictions** 属性 |
| 更改      | Beta    | 向 [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 复杂类型添加了 **userPrincipalName** 和 **sources** 属性 |
| 更改      | Beta    | 向 [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 复杂类型添加了 **userPrincipalName** 和 **sources** 属性 |
| 更改      | Beta    | 将 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性添加到了 [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 复杂类型中 |
| 更改      | Beta    | 从 [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) 复杂类型删除了 **archiveFolder** 属性 |


### <a name="calendar"></a>日历

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | For **findMeetingTimes**, added new enum value **unrestricted** that you specify as the **activityDomain** property, part of the **timeConstraint** parameter. This lets **findMeetingTimes** look for times appropriate for the type of activity you're scheduling for. See details in the [request body](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body) section. |
| 添加项        | Beta          | Support getting an **event** body in plain text, as an alternative to the default HTML format. See [get](/graph/api/event-get?view=graph-rest-beta) and [list](/graph/api/user-list-events?view=graph-rest-beta) events for details. |

### <a name="mail"></a>邮件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta        | Support getting a **message** body in plain text, as an alternative to the default HTML format. See [get](/graph/api/message-get?view=graph-rest-beta) and [list](/graph/api/user-list-messages?view=graph-rest-beta) events for details. |


### <a name="to-do-tasks"></a>待办任务

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 添加新的 **outlook** 导航属性以访问  Outlook 任务。 |
| 添加项        | Beta        | 新实体 [outlookuser](/graph/api/resources/outlookuser?view=graph-rest-beta)、[outlookTaskGroup](/graph/api/resources/outlooktaskgroup?view=graph-rest-beta)、[outlookTaskFolder](/graph/api/resources/outlooktaskfolder?view=graph-rest-beta) 和 [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta) 及其方法支持组织和访问 Outlook 任务。 |
| 添加        | Beta        | Outlook 任务支持附件（[attachment](/graph/api/resources/attachment?view=graph-rest-beta)、[fileAttachment](/graph/api/resources/fileattachment?view=graph-rest-beta)、[itemAttachment](/graph/api/resources/itemattachment?view=graph-rest-beta) 和 [referenceAttachment](/graph/api/resources/referenceattachment?view=graph-rest-beta) 资源）。 |
| 添加项        | Beta        | Outlook 任务支持[扩展的属性](/graph/api/resources/extended-properties-overview?view=graph-rest-beta)（[singleValueLegacyExtendedProperty](/graph/api/resources/singlevaluelegacyextendedproperty?view=graph-rest-beta) 和 [multiValueLegacyExtendedProperty](/graph/api/resources/multivaluelegacyextendedproperty?view=graph-rest-beta) 资源）。 |

### <a name="tasks-and-plans"></a>任务和计划

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 添加了[规划器 API](/graph/api/resources/planner-overview?view=graph-rest-1.0)。<br />新资源：<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-1.0) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-1.0) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-1.0) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-1.0) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-1.0) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-1.0) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-1.0) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-1.0) |

### <a name="sites-and-lists"></a>站点和列表

|**更改类型**|**Version**|**说明**|
|:--------------|:----------|:--------------|
| 添加      | v1.0      | 现在站点的资源在 v1.0 终结点中可用。<br/> 添加了 **site** 和 **siteCollection** 资源类型。
| 更改        | beta 版本      | The format of the identifier for the **site** resource has changed. This is a breaking change in the beta API.
| 已删除       | beta      | The **sharePoint** entity has been removed from the beta API. The functionality is now available from the **sites** collection.

### <a name="sites-and-lists"></a>站点和列表

|**更改类型**|**Version**|**说明**|
|:--------------|:----------|:--------------|
| 更改 | beta 版本 | Removed the **sharepoint** navigation properties. Sites are now accessed directly through the **sites** navigation property. <br/> Removed the **fieldDefinition** resource. It has been replaced by **columnDefinition**. <br/> Removed the **siteCollectionId** and **siteId** properties from **site**. Use **sharepointIds** instead. <br/> Removed the **listItemId** property from **listItem**. Use **sharepointIds** instead. <br/> 将 **listItem** 上的 **columnSet** 属性重命名为 **fields**。 <br/> 更改了 **site** 资源，以将 SharePoint 主机名用作其 ID。
| 加 | beta | 添加了 **booleanColumn**、**calculatedColumn**、**choiceColumn**、**dateTimeColumn**、**lookupColumn**、**numberColumn**、**personOrGroupColumn** 和 **textColumn** 资源类型。 <br/> 向 **site** 添加了 **displayName** 属性。 <br/> 向 **site** 添加了 **columns** 导航属性。 <br/> 向 **sharedDriveItem** 添加了 **list** 和 **listItem** 导航属性。 <br/> 向 **list** 和 **listItem** 以及 **site** 添加了 **sharepointIds** 属性。 <br/> 添加了 **columnDefinition** 资源类型。




## <a name="april-2017"></a>2017 年 4 月

### <a name="identity-and-access--administrative-unit"></a>身份和访问|管理单元

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta        | Adminstrative unit APIs will be updated in preview (beta). The first set of changes will be applied on May 3, 2017. The changes include the following property renaming:<br />scopedRoleMembership 实体的**标识**复杂类型的 - **roleMemberInfo** 复杂类型<br />用户实体的 **scopedRoleMemberOf** 的 - **scopedAdministratorOf** 导航属性<br />administrativeUnit 实体的 **scopedRoleMembers** 的 - **scopedAdministrators** 导航属性<br />directoryRole 实体的 **scopedMembers** 的 - **scopedAdministrators** 导航属性 |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta        | The [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) APIs will be updated in preview (beta). The first set of changes will be applied on May 15, 2017. The changes include property renaming and restructuring. Some properties (such as appRoles and addIns) will not be available until the changes are completed. The changes will be released in preview (beta) prior to releasing to v1.0. |

### <a name="cloud-solution-provider"></a>云解决方案提供商

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | 添加新的预览功能以允许云解决方案提供商预先同意应用程序调用 Microsoft Graph，如新的[授权主题](auth-cloudsolutionprovider.md)中所述。 |

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | 向 [user](/graph/api/resources/user?view=graph-rest-beta) 实体添加了新的 onPremises 属性、onPremisesDomainName、OnPremisesSamAccountName 和 onPremisesUserPrincipalName。 |

### <a name="groups"></a>组

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta        | 向 [Group](/graph/api/resources/group?view=graph-rest-beta) 实体添加了 **HiddenMembership** 作为可见性属性的附加值 |

### <a name="tasks-and-plans"></a>任务和计划

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | 添加了新的[规划器 API](/graph/api/resources/planner-overview?view=graph-rest-beta)。<br />新资源：<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-beta) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-beta) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-beta) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-beta) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-beta) |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | 添加的新实体：<br/>[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-beta)<br/>[deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta)<br/>[deviceManagementScriptGroupAssignment](/graph/api/resources/intune-deviceconfig-devicemanagementscriptgroupassignment?view=graph-rest-beta)<br/>[deviceManagementScriptState](/graph/api/resources/intune-deviceconfig-devicemanagementscriptstate?view=graph-rest-beta)<br/>[eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-beta)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-beta)<br/>[windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-deviceconfig-windowsmanagementapphealthstate?view=graph-rest-beta)<br/> |
| 添加项        | Beta        | 添加的复杂类型：<br/>[dailySchedule](/graph/api/resources/intune-deviceconfig-dailyschedule?view=graph-rest-beta)<br/>[hourlySchedule](/graph/api/resources/intune-deviceconfig-hourlyschedule?view=graph-rest-beta)<br/>[iosBookmark](/graph/api/resources/intune-deviceconfig-iosbookmark?view=graph-rest-beta)<br/>[iosWebContentFilterAutoFilter](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterautofilter?view=graph-rest-beta)<br/>[iosWebContentFilterBase](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterbase?view=graph-rest-beta)<br/>[iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta)<br/>[runSchedule](/graph/api/resources/intune-deviceconfig-runschedule?view=graph-rest-beta)<br/>[sharedAppleDeviceUser](/graph/api/resources/intune-deviceconfig-sharedappledeviceuser?view=graph-rest-beta)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-beta)<br/> |
| 添加        | Beta        | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-beta) 操作 |
| 添加项        | Beta        | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-beta) 操作 |
| 添加        | Beta        | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-beta) 操作 |
| 添加项        | Beta        | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-beta) 操作 |
| 添加项        | Beta        | 在 [deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-deviceconfig-devicemanagementscript-assign?view=graph-rest-beta) 操作 |
| 添加项        | Beta        | 在 [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) 上添加了 [syncLicenses](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-synclicenses?view=graph-rest-beta) 操作 |
| 添加项        | Beta        | 在 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 集合上添加了 **getTopMobileApps** 函数 |
| 添加项        | Beta        | 在 [applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta) 上添加了 [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-deviceconfig-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-beta) 函数 |
| 添加项        | Beta        | 在 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 上添加了 [getDeviceComplianceSettingStates](/graph/api/intune-deviceconfig-devicemanagement-getdevicecompliancesettingstates?view=graph-rest-beta) 函数 |
| 添加项        | Beta        | 在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 上添加了 [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-beta) 函数 |
| 添加项        | Beta        | 在 [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) 上添加了 [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-beta) 函数 |
| 删除        | Beta        | 删除了以下复杂类型：<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/> |
| 更改          | Beta 版本        | 向 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **deviceSharingAllowed** 属性 |
| 更改          | Beta 版本        | 从 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **deviceSharingBlocked** 属性 |
| 更改          | Beta 版本        | 向 [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) 实体添加了 **minimumRequiredSdkVersion** 属性 |
| 更改          | Beta 版本        | 向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **windowsManagementAppEnabled** 属性 |
| 更改          | Beta 版本        | 向 [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) 实体添加了 **notificationTemplateId** 属性 |
| 更改          | Beta 版本        | 向 [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) 实体添加了 **excludeGroup** 属性 |
| 更改          | Beta 版本        | 更改了 [iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-beta) 实体上的以下属性：<br/>将 **payloadFileName** 从必需更改为可选<br/> |
| 更改          | Beta 版本        | 向 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) 实体添加了 **contentFilterSettings** 属性 |
| 更改          | Beta 版本        | 向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **cellularBlockPersonalHotspot** 和 **passcodeBlockFingerprintModification** 属性 |
| 更改          | Beta 版本        | 向 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 实体添加了 **minimumRequiredSdkVersion** 属性 |
| 更改          | Beta 版本        | 更改了 [macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-beta) 实体上的以下属性：<br/>将 **payloadFileName** 从必需更改为可选<br/> |
| 更改          | Beta 版本        | 向 [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) 实体添加了 **disableAppPinIfDevicePinIsSet**、**minimumRequiredOsVersion**、**minimumWarningOsVersion**、**minimumRequiredAppVersion** 和 **minimumWarningAppVersion** 属性 |
| 更改          | Beta 版本        | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **remoteAssistanceSessionUrl**、**isEncrypted**、**model** 和 **manufacturer** 属性 |
| 更改          | Beta 版本        | 更改了 [getMobileAppCount](/graph/api/intune-apps-mobileapp-getmobileappcount?view=graph-rest-beta) 实体上的以下属性：<br/>将 **bindingParameter** 从 **mobileApp** 更改为 *mobileApp* 的**集合**<br/>将 **status** 从 GUID 更改为字符串<br/> |
| 更改          | Beta 版本        | 向 [mobileAppGroupAssignment](/graph/api/resources/intune-apps-mobileappgroupassignment?view=graph-rest-beta) 实体添加了 **vpnConfigurationId** 属性 |
| 更改          | Beta        | 从 [notificationMessageTemplate](/graph/api/resources/intune-deviceconfig-notificationmessagetemplate?view=graph-rest-beta) 实体中删除了 **fromEmailAddress** 属性 |
| 更改          | Beta        | 向 [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) 实体添加了 **excludedApps** 属性 |
| 更改          | Beta 版本        | 从 [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) 实体中删除了 **excludedOfficeApps** 属性 |
| 更改          | Beta 版本        | 向 [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) 实体添加了 **enabled** 属性 |
| 更改          | Beta 版本        | 向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **networkProxyApplySettingsDeviceWide**、**networkProxyDisableAutoDetect**、**networkProxyAutomaticConfigurationUrl**、**networkProxyServer**、**bluetoothDeviceName**、**wiFiScanInterval**、**wirelessDisplayBlockProjectionToThisDevice**、**wirelessDisplayBlockUserInputFromReceiver**、**wirelessDisplayRequirePinForPairing**、**experienceBlockDeviceDiscovery**、**experienceBlockErrorDialogWhenNoSIM**、**experienceBlockTaskSwitcher**、**startMenuPinnedFolderDocuments**、**startMenuPinnedFolderDownloads**、**startMenuPinnedFolderFileExplorer**、**startMenuPinnedFolderHomeGroup**、**startMenuPinnedFolderMusic**、**startMenuPinnedFolderNetwork**、**startMenuPinnedFolderPersonalFolder**、**startMenuPinnedFolderPictures**、**startMenuPinnedFolderSettings**、**startMenuPinnedFolderVideos**、**startMenuAppListVisibility**、**startMenuHideFrequentlyUsedApps**、**startMenuHideRecentJumpLists**、**startMenuHideRecentlyAddedApps**、**startMenuHideRestartOptions**、**startMenuHideUserTile**、**startMenuHidePowerButton**、**startMenuLayoutEdgeAssetsXml**、**personalizationDesktopImageUrl** 和 **personalizationLockScreenImageUrl** 属性 |
| 更改          | Beta 版本        | 更改了 [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **productCode** 从 Guid 更改为字符串<br/> |
| 更改          | Beta 版本        | 更改了 [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) 实体上的以下属性：<br/>将 **phoneProductIdentifier** 从必需更改为可选<br/>将 **phonePublisherId** 从必需更改为可选<br/> |
| 更改          | Beta 版本        | 更改了 [windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta) 实体上的以下属性：<br/>将 **appXPackageInformationList** 从必需更改为可选<br/> |
| 更改          | Beta        | 向 [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta) 实体添加了 **productKey** 和 **licenseType** 属性 |
| 更改          | Beta        | 向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **previewBuildSetting** 属性 |
| 更改          | Beta        | 向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **windowsManagementApp** 和 **managedEBooks** 导航属性 |
| 更改          | Beta        | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **deviceManagementScripts**、**managedDeviceOverview** 和 **cloudPkiSubscriptions** 导航属性 |
| 更改          | Beta        | 向 [deviceEnrollmentPlatformRestrictions](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictions?view=graph-rest-beta) 复杂类型添加了 **osMinimumVersion** 和 **osMaximumVersion** 属性 |
| 更改          | Beta        | 向 [hardwareInformation](/graph/api/resources/intune-deviceconfig-hardwareinformation?view=graph-rest-beta) 复杂类型添加了 **isSharedDevice** 和 **sharedDeviceCachedUsers** 属性 |
| 更改          | Beta        | 更改了 [omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-beta) 复杂类型上的以下属性：<br/>将 **fileName** 从必需更改为可选<br/> |
| 更改          | Beta        | 更改了 [omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-beta) 复杂类型上的以下属性：<br/>将 **fileName** 从必需更改为可选<br/> |

## <a name="march-2017"></a>2017 年 3 月

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加    | Beta    | 添加的新实体：<br/>[androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta)<br/>[androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta)<br/>[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta)<br/>[complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-beta)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta)<br/>[enterpriseCodeSigningCertificate](/graph/api/resources/intune-apps-enterprisecodesigningcertificate?view=graph-rest-beta)<br/>[iosEduDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosedudeviceconfiguration?view=graph-rest-beta)<br/>[managedDeviceCertificateState](/graph/api/resources/intune-devices-manageddevicecertificatestate?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta)<br/>[mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)<br/>[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-beta)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta)<br/>[symantecCodeSigningCertificate](/graph/api/resources/intune-apps-symanteccodesigningcertificate?view=graph-rest-beta)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-beta)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 添加的复杂类型：<br/>[androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationExampleJson](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexamplejson?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-deviceconfig-deviceexchangeaccessstatesummary?view=graph-rest-beta)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-beta)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-beta)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-beta)<br/>[excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta)<br/>[iosEduCertificateSettings](/graph/api/resources/intune-deviceconfig-ioseducertificatesettings?view=graph-rest-beta)<br/>[ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResource](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresource?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-beta)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 在 [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) 上添加了 [requestSignupUrl](/graph/api/intune-androidforwork-androidforworksettings-requestsignupurl?view=graph-rest-beta) 操作 |
| 添加项    | beta    | 在 [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) 上添加了 [completeSignup](/graph/api/intune-androidforwork-androidforworksettings-completesignup?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) 上添加了 [syncApps](/graph/api/intune-androidforwork-androidforworksettings-syncapps?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) 上添加了 [unbind](/graph/api/intune-androidforwork-androidforworksettings-unbind?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 上添加了 [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 上添加了 [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-beta) 操作 |
| Addition    | Beta    | 在 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 上添加了 [removeApplePushNotificationCertificate](/graph/api/intune-onboarding-organization-removeapplepushnotificationcertificate?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 上添加了 [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-iosmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 上添加了 [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-androidmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 上添加了 [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-targetedmanagedappconfiguration-updatemobileappidentifierdeployments?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) 上添加了 [updateTargetedSecurityGroups](/graph/api/intune-mam-iosmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) 上添加了 [updateTargetedSecurityGroups](/graph/api/intune-mam-androidmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) 上添加了 [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta) 上添加了 [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy) 上添加了 [updateTargetedSecurityGroups](/graph/api/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy-updatetargetedsecuritygroups) 操作 |
| 添加项    | Beta    | 在 [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) 上添加了 [wipeManagedAppRegistrationByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationbydevicetag?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 上添加了 [getTopMobileApps](/graph/api/intune-apps-mobileapp-gettopmobileapps?view=graph-rest-beta) 函数 |
| 添加项    | Beta    | 在 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 上添加了 [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-corpenrollment-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-beta) 函数 |
| 删除    | Beta    | 删除了以下实体：<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/> |
| 删除    | Beta    | 删除了以下复杂类型：<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/> |
| 更改      | Beta 版本    | 向 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **webBrowserBlockPopups** 属性 |
| 更改      | Beta 版本    | 从 [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **webBrowserAllowPopups** 属性 |
| 更改      | Beta 版本    | 向 [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta) 实体添加了 **appIdentifier** 属性 |
| 更改      | Beta 版本    | 从 [appReportingOverviewStatus](/graph/api/resources/appreportingoverviewstatus?view=graph-rest-beta) 实体中删除了 **applicationCount**、**failedApplicationCount** 和 **appInstallFailures** 属性 |
| 更改      | Beta 版本    | 向 [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) 实体添加了 **sharedIPadMaximumUserCount** 和 **enableSharedIPad** 属性 |
| 更改      | Beta 版本    | 向 [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) 实体添加了 **shareTokenWithSchoolDataSyncService** 和 **lastSyncErrorCode** 属性 |
| 更改      | Beta 版本    | 向 [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性 |
| 更改      | Beta 版本    | 从 [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) 实体中删除了 **numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime** 和 **policyRevision** 属性 |
| 更改      | Beta 版本    | 向 [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性 |
| 更改      | Beta 版本    | 从 [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) 实体中删除了 **numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime** 和 **policyRevision** 属性 |
| 更改      | Beta 版本    | 向 [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性 |
| 更改      | Beta 版本    | 从 [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) 实体中删除了 **numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime** 和 **policyRevision** 属性 |
| 更改      | Beta 版本    | 向 [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性 |
| 更改      | Beta 版本    | 从 [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) 实体中删除了 **numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime** 和 **policyRevision** 属性 |
| 更改      | Beta 版本    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **subscriptionState** 属性 |
| 更改      | Beta    | 向 [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) 实体添加了 **managedEmailProfileRequired** 属性 |
| 更改      | Beta    | 向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **appsSingleAppModeList** 属性 |
| 更改      | Beta    | 从 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体中删除了 **appsSingleAppModeBundleIds** 属性 |
| 更改      | Beta    | 向 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体添加了 **expirationDateTime** 属性 |
| 更改      | Beta    | 从 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体中删除了 **expiration** 属性 |
| 更改      | Beta    | 向 [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) 实体添加了 **passwordMinimumCharacterSetCount**、**osMinimumVersion**、**osMaximumVersion**、**deviceThreatProtectionEnabled**、**deviceThreatProtectionRequiredSecurityLevel** 和 **storageRequireEncryption** 属性 |
| 更改      | Beta    | 从 [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta) 实体中删除了 **manifest** 属性 |
| 更改      | Beta    | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **isSupervised**、**exchangeLastSuccessfulSyncDateTime**、**exchangeAccessState** 和 **exchangeAccessStateReason** 属性 |
| 更改      | Beta    | 向 [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) 实体添加了 **deviceExchangeAccessStateSummary** 属性 |
| 更改      | Beta    | 从 [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta) 实体中删除了 **manifest** 属性 |
| 更改      | Beta    | 从 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 实体中删除了 **installSummary** 属性 |
| 更改      | Beta    | 向 [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) 实体添加了 **uploadState** 属性 |
| 更改      | Beta    | 更改了 [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) 实体上的以下属性：<br/>将 **azureStorageUriExpirationDateTime** 从必需更改为可选<br/> |
| 更改      | Beta    | 向 [remoteActionAudit](/graph/api/resources/intune-deviceconfig-remoteactionaudit?view=graph-rest-beta) 实体添加了 **initiatedByUserPrincipalName**、**deviceOwnerUserPrincipalName**、**deviceIMEI** 和 **actionState** 属性 |
| 更改      | Beta    | 向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **oneDriveDisableFileSync**、**safeSearchFilter**, **edgeSearchEngine**、**settingsBlockSettingsApp**、**settingsBlockSystemPage**、**settingsBlockDevicesPage**、**settingsBlockNetworkInternetPage**、**settingsBlockPersonalizationPage**、**settingsBlockAccountsPage**、**settingsBlockTimeLanguagePage**、**settingsBlockEaseOfAccessPage**、**settingsBlockPrivacyPage**、**settingsBlockUpdateSecurityPage**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips**、**experienceBlockConsumerSpecificFeatures**、**startMenuLayoutXml**、**startMenuMode**、**logonBlockFastUserSwitching** 和 **startBlockUnpinningAppsFromTaskbar** 属性 |
| 更改      | Beta    | 向 [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) 实体添加了 **allowPrinting**、**allowScreenCapture** 和 **allowTextSuggestion** 属性 |
| 更改      | Beta    | 从 [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) 实体中删除了 **blockPrinting**、**blockScreenCapture** 和 **blockTextSuggestion** 属性 |
| 更改      | Beta    | 向 [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta) 实体添加了 **identityName** 属性 |
| 更改      | Beta    | 更改了 [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **applicableArchitectures** 从 [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) 更改为字符串<br/> |
| 更改      | Beta    | 向 [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) 实体添加了 **identityName** 属性 |
| 更改      | Beta    | 更改了 [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **applicableArchitectures** 从 [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) 更改为字符串<br/> |
| 更改      | Beta    | 向 [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) 实体添加了 **identityName**、**identityPublisherHash** 和 **identityResourceIdentifier** 属性 |
| 更改      | Beta    | 更改了 [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **applicableArchitectures** 从 [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) 更改为字符串<br/>将 **applicableDeviceTypes** 从 [windowsDeviceType](/graph/api/resources/windowsdevicetype?view=graph-rest-beta) 更改为字符串<br/> |
| 更改      | Beta    | 向 [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) 实体添加了 **restartMode** 属性 |
| 更改      | Beta    | 向 [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) 实体添加了 **managedDeviceCertificateStates** 导航属性 |
| 更改      | Beta    | 向 [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta) 实体添加了 **managedDeviceCertificateStates** 导航属性 |
| 更改      | Beta    | 向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **enterpriseCodeSigningCertificates**、**symantecCodeSigningCertificate**、**sideLoadingKeys**、**managedAppPolicies**、**iosManagedAppProtections**、**androidManagedAppProtections**、**defaultManagedAppProtections**、**targetedManagedAppConfigurations**、**mdmWindowsInformationProtectionPolicies**、**windowsInformationProtectionPolicies**、**managedAppRegistrations** 和 **managedAppStatuses** 导航属性 |
| 更改      | Beta    | 从 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体中删除了 **appReportingOverview**、**enterpriseCerts** 和 **symantecCert** 导航属性 |
| 更改      | Beta    | 向 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 实体添加了 **deviceSettingStateSummaries** 导航属性 |
| 更改      | Beta    | 向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 实体添加了 **deviceSettingStateSummaries** 导航属性 |
| 更改      | Beta    | 向 [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) 实体添加了 **termsAndConditions**、**androidForWorkSettings**、**androidForWorkAppConfigurationSchemas**、**applePushNotificationCertificate**、**softwareUpdateStatusSummary**、**deviceCompliancePolicyDeviceStateSummary**、**complianceSettingStateSummaries**、**deviceConfigurationDeviceStateSummaries** 和 **mobileThreatDefenseConnectors** 导航属性 |
| 更改      | Beta    | 从 [iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta) 实体删除了 **teacherRootCertificates**、**teacherIdentityCertificate**、**studentRootCertificates** 和 **studentIdentityCertificate** 导航属性 |
| 更改      | Beta    | 更改了 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **deviceStatuses** 从 [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta) 集合更改为 [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) 集合<br/>将 **groupAssignments** 从 [appProvisioningConfigGroupAssignment](/graph/api/resources/appprovisioningconfiggroupassignment?view=graph-rest-beta) 集合更改为 [mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta) 集合<br/> |
| Change      | Beta    | 向 [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) 实体添加了 **managedDeviceCertificateStates** 导航属性 |
| Change      | Beta    | 向 [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) 实体添加了 **managedDeviceCertificateStates** 导航属性 |
| Change      | Beta    | 向 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体添加了 **deviceConfigurationStates** 和 **deviceCompliancePolicyStates** 导航属性 |
| Change      | Beta    | 向 [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) 实体添加了 **deviceStatusSummary** 和 **userStatusSummary** 导航属性 |
| Change      | Beta    | 向 [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) 实体添加了 **installSummary** 导航属性 |
| Change      | Beta    | 从 [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) 实体中删除了 **sideLoadingKeys** 导航属性 |
| Change      | Beta    | 向 [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) 实体添加了 **managedDeviceCertificateStates** 导航属性 |
| Change      | Beta    | 向 [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta) 实体添加了 **managedDeviceCertificateStates** 导航属性 |
| Change      | Beta    | 从 [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) 复杂类型中删除了 **applicationId**、**appName**、**platformId**、**userFailures** 和 **deviceFailures** 属性 |
| 更改      | Beta    | 向 [iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta) 复杂类型添加了 **displayName** 属性 |
| Change      | Beta    | 向 [iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta) 复杂类型添加了 **displayName** 属性 |
| Change      | Beta    | 向 [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) 复杂类型添加了 **subjectName**、**description**、**expirationDateTime** 和 **certificate** 属性 |
| Change      | Beta    | 从 [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) 复杂类型中删除了 **dataRecoveryCertificate** 和 **certificateFileName** 属性 |
| Change      | Beta    | 向 [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) 复杂类型添加了 **displayName** 属性 |
| Change      | Beta    | 更改了 [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) 复杂类型上以下属性的类型：<br/>将 **applicableArchitecture** 从 [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) 更改为字符串<br/> |
| 更改      | Beta    | 更改了 [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) 复杂类型上的以下属性：<br/>将 **applicableArchitecture** 从可选更改为必需<br/> |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | 新资源：</br>[contract](/graph/api/resources/contract?view=graph-rest-beta) |
| 添加项        | Beta        | 在[域](/graph/api/resources/domain?view=graph-rest-beta)上添加了函数。<br/>新实体：</br>[domain](/graph/api/resources/domain?view=graph-rest-beta)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-beta)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-beta)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-beta)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-beta)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-beta)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-beta)<br/>新操作：</br>[forceDelete](/graph/api/domain-forcedelete?view=graph-rest-beta)</br>[verify](/graph/api/domain-verify?view=graph-rest-beta) |

### <a name="schema-extensions"></a>架构扩展

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | Extend Microsoft Graph with application data by using [schema extensions](extensibility-overview.md#schema-extensions).  This is supported on the following resources:<br/>管理单元<br/>日历事件<br/>设备<br/>组<br/>message<br/>组织<br/>个人联系人<br/>帖子<br/>用户<br/>请参阅以下示例：<br/>[使用架构扩展向组添加自定义数据（预览）](extensibility-schema-groups.md) |
| 添加项        | Beta        | Provided an alternative way to create a schema extension definition without requiring a verified .com vanity domain. See [schema extensions](extensibility-overview.md#schema-extensions) for details. |

### <a name="open-extensions"></a>开放扩展

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改          | v1.0 和 beta | 将前述“Office 365 数据扩展”重命名为“开放扩展”。 |
| 添加项        | Beta          | 已添加支持[开放扩展](extensibility-overview.md#open-extensions)的资源： <br/>管理单元<br/>设备<br/>group<br/>组织<br/>用户<br/>请参阅以下示例：<br/>[使用开放扩展向用户添加自定义数据（预览）](extensibility-open-users.md) |

### <a name="identity-and-access"></a>身份和访问

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 已添加对[还原并永久删除组](/graph/api/resources/directory?view=graph-rest-beta)的支持。<br/>新实体：带有 deleteditems 导航属性的目录。 |
| 添加项        | Beta        | 新实体：</br>[终结点](/graph/api/resources/endpoint?view=graph-rest-beta) |
| 更改          | Beta        | 针对[组](/graph/api/resources/group?view=graph-rest-beta)的新 [endpoints](/graph/api/group-list-endpoints?view=graph-rest-beta) 导航属性 |
| 添加项        | Beta        | 新实体：</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-beta) |
| 更改          | Beta        | 针对[用户](/graph/api/resources/user?view=graph-rest-beta)的新 [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-beta) 导航属性 |
| 添加项        | Beta        | 新实体：</br>[contract](/graph/api/resources/contract?view=graph-rest-beta) |

### <a name="reports"></a>报告

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Introduced the new preview API for Office 365 Reports. You can use it to get usage reports of how people in your business are using Office 365 services. For example, you can identify who is using a service a lot and reaching quotas, or who may not need an Office 365 license at all. For more details, see [report](/graph/api/resources/report?view=graph-rest-beta). |


## <a name="february-2017"></a>2017 年 2 月

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| 更改类型 | 版本 | 说明                              |
| :---------- | :------ | :--------------------------------------- |
| 添加项    | Beta    | 增加了新实体：<br/>[androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)<br/>[androidForWorkEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkeasemailprofilebase?view=graph-rest-beta)<br/>[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidForWorkGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgmaileasconfiguration?view=graph-rest-beta)<br/>[androidForWorkNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworknineworkeasconfiguration?view=graph-rest-beta)<br/>[androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)<br/>[androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)<br/>[androidForWorkTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidforworktrustedrootcertificate?view=graph-rest-beta)<br/>[androidForWorkWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkwificonfiguration?view=graph-rest-beta)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-beta)<br/>[appProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-appprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)<br/>[enterpriseCertificate](/graph/api/resources/intune-apps-enterprisecertificate?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)<br/>[symantecCertificate](/graph/api/resources/intune-apps-symanteccertificate?view=graph-rest-beta)<br/>[windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)<br/>[windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)<br/>[windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)<br/>[windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta)<br/>[windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 新增了复杂类型：<br/>[airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta)<br/>[windowsArchitecture](/graph/api/resources/intune-apps-windowsarchitecture?view=graph-rest-beta)<br/>[windowsDeviceType](/graph/api/resources/intune-apps-windowsdevicetype?view=graph-rest-beta)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta)<br/> |
| 添加项    | Beta    | 在 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体上添加了 [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 实体上添加了 [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体上添加了 [updateTargetedSecurityGroups](/graph/api/intune-mam-targetedmanagedappconfiguration-updatetargetedsecuritygroups?view=graph-rest-beta) 操作 |
| 添加项    | Beta    | 在 [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) 实体上添加了 [getScopesForUser](/graph/api/intune-rbac-resourceoperation-getscopesforintune-devices-user?view=graph-rest-beta) 函数 |
| 更改      | Beta    | 从 [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta) 实体中删除了 **manifest** 属性 |
| 更改      | Beta    | 向 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) 实体添加了 **assetTagTemplate****lockScreenFootnote****homeScreenDockIcons** 和 **homeScreenPages** 属性 |
| 更改      | Beta    | 从 [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) 实体删除了 **deviceSharingAssetTagInformation**、**deviceSharingLockScreenFootnote**、**homeScreenLayoutDockIcons** 和 **homeScreenLayoutPages** 属性 |
| 更改      | Beta    | 向 [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) 实体添加了 **appsSingleAppModeBundleIds** 属性 |
| 更改      | Beta    | 从 [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta) 实体删除了 **manifest** 属性 |
| 更改      | Beta    | 向 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体添加了 **createdDateTime**、**description**、**lastModifiedDateTime**、**displayName** 和 **version** 属性 |
| 更改      | Beta    | 向 [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) 实体添加了 **createdDateTime** 和 **lastModifiedDateTime** 属性 |
| 更改      | Beta    | 从 [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) 实体删除了 **deviceRegistrationState** 属性 |
| 更改      | Beta    | 向 [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) 实体添加了 **manifest** 属性 |
| 更改      | Beta    | 向 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) 实体添加了 **osDescription** 和 **userName** 属性 |
| 更改      | Beta    | 从 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) 实体删除了 **deviceType** 属性 |
| 更改      | Beta    | 更改了 [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) 实体以下属性的类型：<br/>将 **mobileAppInstallStatusValue** 从 Int32 更改为字符串 |
| 更改      | Beta    | 向 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体添加了 **targetedSecurityGroupIds** 和 **targetedSecurityGroupsCount** 属性 |
| 更改      | Beta    | 从 [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) 实体删除了 **numberOfTargetedSecurityGroups** 属性 |
| 更改      | Beta    | 向 [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) 实体添加了 **id** 属性 |
| 更改      | Beta    | 从 [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta) 实体删除了 **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue** 和 **certificateValidityPeriodScale** 属性 |
| 更改      | Beta    | 从 [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta) 实体删除了 **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue** 和 **certificateValidityPeriodScale** 属性 |
| 更改      | Beta    | 从 [windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-beta) 实体删除了 **applyToWindows10Mobile** 属性 |
| 更改      | Beta    | 向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 实体添加了 **enterpriseCerts**、**iosLobAppProvisioningConfigurations** 和 **symantecCert** 导航属性 |
| 更改      | Beta    | 向 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 实体添加了 **userStatusOverview** 导航属性 |
| 更改      | Beta    | 向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 实体添加了 **userStatusOverview** 导航属性 |
| 更改      | Beta    | 向 [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) 实体添加了 **groupAssignments**、**deviceStatuses** 和 **userStatuses** 导航属性 |
| 更改      | Beta    | 更改了 [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) 实体上以下属性的类型：<br/>将 **identityCertificate** 从 [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta) 更改为 [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta) |
| 更改      | Beta    | 向 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型添加了 **deviceComplianceCheckinThresholdDays** 和 **isScheduledActionEnabled** 属性 |
| 更改      | Beta    | 从 [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 复杂类型删除了 **windowsCommercialId** 和 **windowsCommercialIdLastModifiedTime** 属性 |
| 更改      | Beta    | 向 [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta) 复杂类型添加了 **bundleID**、**appName**、**publisher**、**enabled** 和 **showOnLockScreen** 属性 |
| 更改      | Beta    | 从 [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta) 复杂类型删除了 **bundleIdentifier**、**notificationsEnabled** 和 **showInLockScreen** 属性 |



## <a name="january-2017"></a>2017 年 1 月

### <a name="calendar"></a>日历

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | [用户](/graph/api/resources/user?view=graph-rest-1.0)资源的新操作 [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)。 |
| 添加项        | v1.0        | 新复杂类型 [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-1.0)，由 attendee 类型的类型属性组成。 |
| 添加项        | v1.0        | 新复杂类型：<br/>[attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-1.0)<br/>[locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-1.0) <br/>[locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-1.0)<br/>[meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-1.0)<br/>[meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-1.0)<br/>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-1.0)<br/>[timeSlot](/graph/api/resources/timeslot?view=graph-rest-1.0) |
| 更改          | v1.0        | The [attendee](/graph/api/resources/attendee?view=graph-rest-1.0) complex type is now derived from attendeeBase, which in turn is derived from [recipient](/graph/api/resources/recipient?view=graph-rest-1.0). Including the inherited properties, it consists of the same **status**, **type** and **emailAddress** properties as before. |
| 添加项        | Beta        | 添加到[日历](/graph/api/resources/calendar?view=graph-rest-beta)资源的 hexColor。 |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加的新实体： <br/>[appReportingOverviewStatus](/graph/api/resources/intune-apps-appreportingoverviewstatus?view=graph-rest-beta)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)<br/>[deviceManagementExchangeOnpremisesPolicy](/graph/api/resources/intune-onboarding-devicemanagementexchangeonpremisespolicy?view=graph-rest-beta)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)<br/>[onpremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-beta)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)<br/>[windows10WindowsInformationProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10windowsinformationprotectionconfiguration?view=graph-rest-beta) |
|添加项|Beta|新增了复杂类型： <br/> [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta)<br/>[enterpriseCloudResource](/graph/api/resources/intune-deviceconfig-enterprisecloudresource?view=graph-rest-beta)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-beta)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-beta)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-beta)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta)<br/>[iPv6Range](/graph/api/resources/intune-deviceconfig-ipv6range?view=graph-rest-beta)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRule](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprule?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruleapplockerpolicyfiletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruledesktoptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprulestoreapptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionCorporateNetworkLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectioncorporatenetworklocation?view=graph-rest-beta)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocation?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisecloudresources?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv4ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv6ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationneutralresources?view=graph-rest-beta)
|删除|Beta|删除了以下复杂类型，并替换为 microsoft.graph.Json：<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|更改|Beta 版本|已将以下实体的属性类型从 appConfigComplianceStatus 替换为 complianceStatus： <br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta)|
|Change|Beta|对于资源 [managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-beta)，已将属性内容的类型从 managedAppSummary 更改为 Json。|
|Change|Beta 版本|从 [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) 集合中删除了 getUsersWithFlaggedAppRegistration 函数。|
|Change|Beta 版本|已将 [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) 实体的 **vppToken** 导航属性更改为不再是包含的集合。|
|Change|Beta 版本|向 [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) 和 [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) 实体添加了 **deviceStatusOverview** 属性。|
|Change|Beta 版本|向 [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) 单一实例添加了 **appReportingOverview** 属性。|
|Change|Beta 版本|向 [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta)、[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) 和 [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) 实体添加了 **deviceDisplayName** 和 **userPrincipalName** 属性。|
|Change|Beta 版本|向 [deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-beta) 实体添加了 **ruleName** 属性。|
|Change|Beta 版本|向 [deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-beta)、[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-beta) 和 [managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta) 实体添加了 **devicesCount**、**userDisplayName** 和 **userPrincipalName** 属性。|
|Change|Beta 版本|向 [deviceManagement](/graph/api/resources/intune-deviceconfig-devicemanagement?view=graph-rest-beta) 单一实例添加了 [notificationMessageTemplates](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) 集合。|
|Change|Beta 版本|向 [localizedNotificationMessage](/graph/api/resources/intune-deviceconfig-localizednotificationmessage?view=graph-rest-beta) 实体添加了 **isDefault**、**lastModifiedDateTime**、**locale**、**messageTemplate** 和 **subject** 属性。|
|Change|beta|向 [managedDevice](/graph/api/resources/intune-onboarding-manageddevice?view=graph-rest-beta) 实体添加了 **azureActiveDirectoryDeviceId**、**deviceCategory**、**deviceRegistrationState** 和 **managementAgent** 属性。|
|更改|beta|向 [mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-beta) 实体添加了 **lastModifiedDateTime** 属性。|
|更改|Beta|向 [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) 实体添加了 **brandingOptions**、**defaultLocale**、**displayName**、**fromEmailAddress**、**lastModifiedDateTime** 和 **localizedNotificationMessages** 属性。|
|更改|beta|向 [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) 实体添加了 **appsAllowTrustedAppsSideloading**、**appsBlockWindowsStoreOriginatedApps**、**developerUnlockSetting**、**edgeBlockAccessToAboutFlags**、**edgeBlockDeveloperTools**、**edgeBlockExtensions**、**edgeBlockInPrivateBrowsing**、**edgeFirstRunUrl**、**edgeHomepageUrls**、**gameDvrBlocked**、**settingsBlockAddProvisioningPackage**、**settingsBlockChangeLanguage**、**settingsBlockChangePowerSleep**、**settingsBlockChangeRegion**、**settingsBlockChangeSystemTime**、**settingsBlockEditDeviceName**、**settingsBlockRemoveProvisioningPackage**、**sharedUserAppDataAllowed**、**smartScreenBlockPromptOverride**、**smartScreenBlockPromptOverrideForFiles**、**storageRestrictAppDataToSystemVolume** 、**storageRestrictAppInstallToSystemVolume** 、**webRtcBlockLocalhostIpAddress**、**windowsStoreBlockAutoUpdate** 和 **windowsStoreEnablePrivateStoreOnly** 属性。|

## <a name="december-2016"></a>2016 年 12 月

### <a name="change-tracking"></a>更改跟踪

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 将新的 delta 函数添加到以下实体，以执行[delta 查询](delta-query-overview.md)：<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>有关示例，请参阅以下文章：<br/>[获取组的增量更改（预览）](delta-query-groups.md)<br/>[获取文件夹中邮件的增量更改（预览）](delta-query-messages.md)<br/>[获取用户的增量更改（预览）](delta-query-users.md) |

### <a name="workbooks-and-charts"></a>工作簿和图表

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 添加了 workbookPivotTable 资源；数据透视表上的 refresh 和 refreshAll 操作；workbookRangeView 资源；已筛选的范围上的 visibleView 操作，可向用户返回 workbookRangeView；从 visibleView 中删除了 rows 集合和 range 资源；从 range 资源中删除了 columnsAfter、columnsBefore、resizedRange、rowsAbove、rowsBelow 函数；新增表属性。 |

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Added resources and method APIs for Microsoft Intune. This is a large set of resources and methods to support the public preview of Intune on Azure Portal. For information about the Intune service, see the [Intune documentation](https://go.microsoft.com/fwlink/?linkid=836405). For information about the Intune resources and APIs, see [Working with Intune in Microsoft Graph](/graph/api/resources/intune-graph-overview?view=graph-rest-beta). |

## <a name="october-2016"></a>2016 年 10 月

### <a name="authorization-provider"></a>授权提供程序

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | v2.0 授权终结点现在支持 client_credentials OAuth 授权哪些添加项可以用于[业务方案中的守护程序和长时间运行的进程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。 |
| 添加项        | v1.0 和 beta | v2.0 授权终结点现在通过[管理员同意终结点](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions)支持[需要征得管理员同意的权限范围](permissions-reference.md)。 |
| 添加项        | v1.0 和 beta | v2.0 授权终结点现在通过[管理员同意终结点](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions)支持对租户中的所有用户授予管理员同意。 |

### <a name="identity-and-access--invitation-manager"></a>身份和访问|邀请管理器

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向邀请实体类型添加了 invitedUserType 属性，用于定义受邀用户类型（**来宾**或**成员**）。 |
| 删除        | Beta        | We will be removing the invitedToGroups property from the invitation entity-type on 11/11/2016. This means that you will no longer be able to add an invited user to a group using this API. Instead, use the [add member API](/graph/api/group-post-members?view=graph-rest-1.0) to add a user to a group. |

## <a name="september-2016"></a>2016 年 9 月

### <a name="identity-and-access--application"></a>身份和访问|应用程序

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Azure AD Application Proxy APIs are now available in the Microsoft Graph beta endpoint. These APIs allow for secure publishing of on-premises applications to users outside the corporate network using Azure AD as the common control plane for access. You can use the published APIs to write applications that can retrieve and update various aspects of application proxy, such as _connectors_, _connectorGroups_ and the _onPremisesPublishing_ settings of an application. |

### <a name="files"></a>文件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加了 shared 集合以允许按 shareId 或共享 URL 访问共享的 driveItem。 |
| Addition        | Beta        | 向驱动器添加了 _search_ 函数，允许搜索驱动器根文件夹之外的更多项。 |
| 添加项        | Beta        | 添加了对 createUploadSession 的支持，可允许将大于 4 MB 的文件上载到 OneDrive、OneDrive for Business 和 SharePoint 文档库。 |
| 添加项        | Beta        | 向 driveItem 添加了 sharepointIds 属性，可返回 SharePoint 中存储的 driveItem 的传统 SharePoint API 标识符。 |
| 添加项        | Beta        | 在 remoteItem 上添加了其他属性。 |
| 添加项        | Beta        | 为 OneDrive for Business 中的文件添加了 quickXorHash 值。 |
| 添加项        | Beta        | 添加了 createSharingLink 的作用域以允许创建企业共享链接或匿名共享链接。 |

### <a name="calendar-groups-mail-personal-contacts"></a>日历、组、邮件、个人联系人

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 目前以下资源支持[扩展属性](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0)：message、mailFolder、event、calendar、contact、contactFolder、group event、group calendar、group post。 |

### <a name="groups"></a>组

通过公共预览 API 添加了对动态组成员身份的支持，包括下表中列出的添加项。

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 添加了 **membershipRule** 属性，如果此组是动态组，则该属性会包含控制该组的成员资格的规则。 |
| 添加项        | Beta        | 添加了 **membershipRuleProcessingState** 属性以控制是否对该组启用或暂停动态组成员资格处理。 |
| 添加项        | Beta        | 设置了 **groupTypes** 属性以包含 **“DynamicMembership”** 来表明该组的动态组功能。 |
| 添加项        | Beta        | 添加了 **preferredLanguage** 属性以指示 Office 365 组的首选语言。 |
| 添加项        | Beta        | 添加了 **theme** 属性以指定 Office 365 组的颜色主题。 |

### <a name="hybrid-deployment"></a>混合部署

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | Apps can use v1.0 Outlook Mail, Calendar, and Contacts APIs to access on-premises mailboxes in a hybrid deployment with Exchange 2016 Cumulative Update 3 (CU3). Find more details about REST API support in specific [hybrid deployments](hybrid-rest-support.md). **Note:** If you're using these sets of API in v1.0, you can now find your apps, including production apps, working for on-premises mailboxes that meet the specific hybrid deployment requirements. This capability is only in preview. |

### <a name="identity-and-access--identity-protection"></a>身份和访问 | 身份保护

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta        | 作为架构更改的一部分，两个位置属性的类型将在 identityRiskEvents 终结点中替换为新的复杂类型，将在 identityRiskEvents 终结点中更改/添加以下属性：</br>**location** 已从 Edm.String 更改为 ComplexType signInLocation。<br/>**previousLocation** 已从 Edm.String 更改为 ComplexType signInLocation。<br/>**signInLocation** 是新的 ComplexType，其中包含 city、state、countryOrRegion 和 geoCoordinates 属性。<br/>**geoCoordinates** 是新的 ComplexType，其中包含 latitude 和 longitude 属性。 |

### <a name="identity-and-access--invitation-manager"></a>身份和访问|邀请管理器

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Invitation manager APIs are now available in the Microsoft Graph beta endpoint. You can use invitation manager APIs to create an invite, in order to add an external user to the organization. As part of the invitation, you can also choose to add the invited user to an Office 365 group. For more details, see [invitation manager](/graph/api/resources/invitation?view=graph-rest-beta). |

### <a name="files"></a>文件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 在 **driveItem** 上添加了 **CreateUploadSession** 方法，可支持大型文件和可恢复上载。 |
| 添加项        | v1.0        | 在 SharePoint 中的项目上添加了用于跟踪 SharePoint ID 的属性 (**sharepointIds**) 以及用于标识根文件夹的属性 (**root**)。 |
| 添加项        | v1.0        | Added **Shares** root collection, which can be used with shareIds or sharing links to access shared items in OneDrive and SharePoint. Returns a new type, sharedDriveItem. |
| 添加项        | v1.0        | 在 driveItem 上添加了 **Invite** 方法，可允许向项目添加权限。 |
| 添加项        | v1.0        | 在驱动器上添加了 **Search** 方法，可允许搜索驱动器中的项目和共享项目。 |
| 添加项        | v1.0        | 在哈希复杂类型上的文件复杂类型 quickXorHash 属性上添加了 **processingMetadata** 属性。 |
| 添加项        | v1.0        | 在哈希复杂类型上添加了 **quickXorHash** 属性 |

### <a name="calendar"></a>日历

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 向 [event](/graph/api/resources/event?view=graph-rest-1.0) 资源添加了 **onlineMeetingUrl** 属性。 |
| 添加项        | Beta        | 向事件资源添加了 [forward](/graph/api/event-forward?view=graph-rest-beta) 操作。 |
| 添加项        | Beta        | 向[日历](/graph/api/resources/calendar?view=graph-rest-beta)资源添加了以下属性以支持日历共享：**canEdit**、**canShare**、**canViewPrivateItems**、**isShared**、**isShareWithMe** 和 **owner**。 |

### <a name="change-notifications"></a>更改通知

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 将驱动器根项作为可供订阅的资源添加到了 Webhook。 |

### <a name="mail"></a>邮件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Added support for creating, listing, getting, and deleting one or more instances of [mention](/graph/api/resources/mention?view=graph-rest-beta) in a message. Mentions support calling out to get the attention of other users in a message. |
| 添加项        | Beta        | 添加了对 [getMailTips](/graph/api/user-getmailtips?view=graph-rest-beta) 操作的支持，可以获取特定收件人的所有邮件提示。 添加了以下资源：[automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-beta)、[mailTips](/graph/api/resources/mailtips?view=graph-rest-beta)、[mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-beta)。 |

### <a name="query-parameters"></a>查询参数

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta        | 自 2016 年 9 月 26 日起，支持不含 $ 前缀的查询参数。 在查询参数中，$ 前缀是可选的。 |

### <a name="sites-and-lists"></a>站点和列表

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | [按照 ID](/graph/api/list-get?view=graph-rest-beta) 或[路径/URL](/graph/api/baseitem-getbyurl?view=graph-rest-beta) 访问 SharePoint 网站和列表。 |
| 添加项        | Beta        | 支持[列出、创建、获取和删除 listItem 实例](/graph/api/resources/listitem?view=graph-rest-beta)。 |

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Added **refreshTokensValidFromDateTime** read-only property to indicate when refresh or session tokens are valid from. Any tokens issued before this time are invalid, and any attempt to use them would force a new sign-in for the user. |
| 添加项        | Beta        | 添加了 **showInAddressList** 属性来控制 Outlook 全局地址列表是否应包含此用户。 |
| 添加项        | Beta        | 添加了 **invalidateAllRefreshTokens** 服务操作，可通过将 **refreshTokensValidFromDateTime** 用户属性重置为当前的日期时间来使向应用程序颁发的用户的所有刷新和会话令牌失效。 |

### <a name="users--outlook-settings"></a>用户|Outlook 设置

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | 添加了 [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) 复杂类型，其中包括 **automaticRepliesSetting**、**timeZone** 和 **language** 属性。 |
| 添加项        | v1.0        | 向 [user](/graph/api/resources/user?view=graph-rest-1.0) 资源添加了 **mailboxSettings** 属性。 |


## <a name="august-2016"></a>2016 年 8 月

### <a name="personal-contacts"></a>个人联系人

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | As part of the schema change where a few properties are being removed and corresponding collections are being added to contacts endpoint, the following properties have been added to the contacts endpoint: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. For details, see the [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/) blog post. |
| 删除        | Beta        | As part of the schema change where a few properties are being removed and corresponding collections are being added to contacts endpoint, the following properties have been removed from the contacts endpoint: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. For details, see the [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/) blog post. |

### <a name="workbooks-and-charts"></a>工作簿和图表 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加项        | v1.0        | Excel REST API on Microsoft Graph is generally available. Now you can build rich and deep integrations with Excel workbooks in Office 365. See the [Power your apps with the new Excel REST API on the Microsoft Graph](https://developer.microsoft.com/office/blogs/power-your-apps-with-the-new-excel-rest-api/) blog post for more details. |

### <a name="social-and-workplace-intelligence--people"></a>社交和工作场所智能 | 人员

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 更改          | Beta 版本        | Property _WebSite_ is renamed to _Websites_. For details, see [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="identity-and-access--privileged-identity-management"></a>身份和访问|特权身份管理

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Privileged Identity Management (PIM) REST APIs now are available in the Microsoft Graph beta endpoint. [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) provides just in time activation for privileged Azure AD organizational roles such as Global Administrator, Billing Administrator, and so on. You can use the published APIs to write applications that retrieve and update privileged role assignments, and activate users into roles. For details, see [Microsoft Graph: Azure AD Privileged Identity Management Preview APIs available in Beta](https://developer.microsoft.com/office/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta/) and [Azure AD Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta). |

## <a name="july-2016"></a>2016 年 7 月

### <a name="identity-and-access--administrative-unit"></a>身份和访问|管理单元

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | Introduced the new Administrative Unites preview API. Administrative units allow organizations to subdivide their Azure Active Directory, and delegate administrative duties to those subdivisions. Subdivisions can represent regions, departments, cost centers, etc. This can now be managed through the Microsoft Graph API. |

## <a name="june-2016"></a>2016 年 6 月

### <a name="identity-and-access--identity-protection"></a>身份和访问 | 身份保护

|**更改类型**|**Version**|**说明**|
|:--------------|:-----------|:--------------|
|添加|Beta|Introduced the new IdentityRiskEvents preview API. This API works in conjunction with Azure Active Directory Identity Protection. You can use it to query risk events generated by Identity Protection. For more details, see the [Introduction of a new preview API to Microsoft Graph: IdentityRiskEvents](https://developer.microsoft.com/office/blogs/identityriskevents-api-preview/) blog post.

### <a name="change-notifications"></a>更改通知

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | mail 和 contacts 订阅现在支持仅应用作用域。 |

## <a name="may-2016"></a>2016 年 5 月

### <a name="calendar"></a>日历

|**更改类型**|**Version**|**说明**|
|:--------------|:-----------|:--------------|
|重大更改|Beta|针对 findMeetingTimes API 的更改。 有关详细信息，请参阅 [Microsoft Graph findMeetingTimes API 更新](https://developer.microsoft.com/graph/blogs/microsoft-graph-findmeetingtimes-api-update/)博客文章。 此更改于 2016 年 5 月 19 日生效。

### <a name="personal-contact"></a>个人联系人 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 添加了 extensions，它是用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。 |

### <a name="identity-and-access--directory-setting"></a>身份和访问|目录设置

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 重大更改 | Beta        | _settingTemplateId_ is renamed to _templateId_. This change will take effect May 19th, 2016. |

### <a name="calendar"></a>日历 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 向**事件**实体添加了_扩展_, 它是用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。 |
| 添加项        | v1.0        | 向**eventMessages**实体添加了_inferenceClassification_和_扩展_。 |
| 添加项        | Beta        | 向**eventMessageRequest**实体添加了_responseRequested_。 |

### <a name="mail"></a>邮件 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 向**message**实体添加了_inferenceClassification_和_扩展_。 |

### <a name="personal-contacts"></a>个人联系人 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 将 _wellknownname_ 添加到 **contactFolder**实体。 |

### <a name="groups"></a>组

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 向**post **实体添加了_扩展_，它是用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。 |

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 添加了 inferenceClassification 资源类型。 |
| 添加        | beta        | 向 mailboxsettings 添加了 timeZone。   |
| Addition        | beta        | 向 _user_ 添加了 API _findMeetingTimes_to。   |

## <a name="april-2016"></a>2016 年 4 月

### <a name="general"></a>常规

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加项        | v1.0 和 Beta | 添加了遵守 Accept-Encoding:gzip 的支持。 |
| 新增        | v1.0          | Added support for cast segment in expand path. For example, 'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event'. |
| 添加        | beta          | Added support for PATCH request against structural properties. For example: 'PATCH /me/mailboxSettings'. |
| 添加        | beta          | Azure Active Directory is now used as a fallback for /beta/users/id/photo requests when Outlook is unable to service the request, for example when the user has no mailbox license or the tenant does not have an Exchange Online subscription. NOTE: this fallback is available for both GET and PATCH. |
| 添加        | beta          | Added support for cast segment in expand path. For example: 'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event'. |

### <a name="files"></a>文件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 修补程序             | v1.0        | 修复了出现 500 和“不支持的扩展属性类型”故障的 OneDrive createLink 请求问题。 |

## <a name="march-2016"></a>2016 年 3 月

### <a name="calendar"></a>日历

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | beta        | 添加了 singleValueExtendedProperties 和 multiValueExtendedProperties 属性。 |
| 添加        | beta        | 向 _meetingTimeCandidate_ 添加了 _suggestionHint_ 属性。 |
| 添加        | beta        | 向 location 添加了 locationUri 属性。 |
| 添加        | beta        | 向 _physicalAddress_ 添加了_type_ 和 _postOfficeBox_。 |
| 更改          | Beta 版本        | findMeetingTimes 现在采用了新参数 ReturnSuggestionHints。 |
| 更改          | Beta        | findMeetingTimes 现在返回 meetingTimeCandidate 的集合。 |

### <a name="files"></a>文件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | Added _recent_ function to list a set of items that have been recently used by the signed in user. This list includes items that are in the user's drive as well as items they have access tofrom other drives. Example: GET /me/drive/recent. |
| 添加项        | v1.0 和 beta | Added _sharedWithMe_ function to list the set of items that are shared with the current user. Example: GET /me/drive/sharedWithMe. |
| 添加项        | v1.0 和 beta | 添加了 remoteItem 类型以提供指向其他驱动器中的项目的链接。 |
| 添加项        | v1.0 和 beta | 添加了 sharingInvitation 类型以提供此权限关联的任何共享邀请的详细信息。 |
| 添加项        | v1.0 和 beta | Added _delta_ function to track changes to items in a drive. Example: GET /me/drive/items/{item-id}/delta |
| 添加项        | v1.0 和 beta | Added _copy_ that creates a copy of a _driveItem_ (including any children), under a new parent or with a new name. Example: POST /me/drive/items/{item-id}/copy. |
| 添加项        | v1.0 和 beta | conflictBehavior 实例属性现在适用于 driveItem。 |
|添加项|Beta|Added _invite_ function to send a sharing invitation to an existing item. A sharing invitation creates a unique sharing link and sends an email to the recipient of the invitation that includes the sharing link. Example: POST /drive/items/{item-id}/invite.

### <a name="calendar"></a>日历

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向**事件**实体添加了新属性_onlineMeetingUrl_和新方法_Cancel_。 |
| 添加项        | Beta        | 向**eventMessage**实体添加了_startDateTime_、_endDateTime_、_location_、 _type_、_recurrence_、_isOutOfDate_、_conversationIndex_、_unsubscribe_、_unsubscribeData_、_unsubscribeEnabled_ 和 _flag_属性。 |
| 添加项        | Beta        | 向**eventMessage**实体添加了_singleValueExtendedProperties_和_multiValueExtendedProperties_属性。 |
| 添加项        | Beta        | 添加了_取消订阅_ **eventMessage**实体的新方法。|

### <a name="workbooks-and-charts"></a>工作簿和图表

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | We are adding new Excel REST APIs that let you read and modify data in an Excel workbook. It is now possible to build smart apps that allows users to get value out of the content stored in an Excel workbook by providing insights into the data. Take advantage of analytical powers of Excel, create tables and charts and extract visually appealing chart image - all from within your app. For details, see [Working with Excel in Microsoft Graph](/graph/api/resources/excel?view=graph-rest-beta). |

### <a name="general"></a>常规

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | 改进了解析租户别名和拒绝的 JWT (AAD) 令牌时出现的错误消息。 |
| 添加项        | v1.0 和 beta | 收到含有空持有者令牌的请求时，在 www-authenticate 标头中现在返回授权服务终结点的位置。 |
| 添加项        | v1.0 和 beta | The ability to filter on an entity's id property is now fixed. Example: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Previously, any POST requests to service actions and functions require prefixing the action or function name with the microsoft.graph prefix. For example: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups.<br/>The prefix is now no longer required (although it can still be specified). So the following would now also work: POST https://graph.microsoft.com/v1.0/me/getMemberGroups. |
| 更改          | Beta          | 清理了订阅属性名称。  |
| 添加项        | Beta          | We've added the capability to discover (through _directorySettingTemplates_) and override the default behavior (by creating a _setting_ from the template) for entities and their associated functionality. Initially this only template provided is to control behaviors on Office groups. |

### <a name="mail"></a>邮件

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向**mailFolder**实体添加了_wellKnownName_ 和_userConfigurations_属性。 |
| 添加项        | Beta        | 向**mailFolder**实体添加了_singleValueExtendedProperties_和_multiValueExtendedProperties_属性。 |
| 添加项        | v1.0          | 向 **message** 实体添加了 _mobilePhone_属性。            |
| 添加项        | v1.0 和 beta | 向 **message** 实体添加了 _internetMessageId_属性。 由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。 |F>>
| 更改          | Beta          | 将**message**实体中的_ mobilePhone1_属性重命名为_mobilePhone_。 |
| 更改          | Beta          | **message** 实体的_createReply_ 和_createReplyAll_ 采用了新参数：_Message_和 _comment_。 |
| 更改          | Beta          | **message**实体的_createForward_ 采用了新参数：_Message_、_ToRecipients_ 和 _comment_。 |
| 更改          | Beta          | **message**实体的_reply_、_replyAll_ 和 _forward_ 采用了新参数_Message_。 |

### <a name="permission"></a>权限

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | 添加了 sharingInvitation 属性以提供此权限关联的任何共享邀请的详细信息。 |

### <a name="social-and-workplace-intelligence--people"></a>社交和工作场所智能|人员

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta 版本        | 添加了新属性：birthday、personNotes、isFavorite、phones、permission、postalAddresses、websites、yomiCompany、department、profession、mailboxType 和 personType。 |
| 添加项        | Beta 版本        | 添加了以下新枚举类型：_physicalAddressType_、_webSite_、_phone_ 和 _webSiteType_。 |

### <a name="calendar-group-mail-to-do-tasks"></a>日历、群组、邮件、待办任务

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta        | 向 _referenceAttachment_ 实体添加了新属性 _sourceUrl_、_providerType_、_thumbnailUrl_、_previewUrl_、_permission_ 和 **isFolder**。 （参考附件在 **event**、**message**、**outlookTask**或**post**中受到支持。）  |
| 添加项        | Beta        | 向**referenceAttachment**实体添加了_singleValueExtendedProperties_和_multiValueExtendedProperties_属性。 |
| 添加项        | Beta 版本        | 添加了以下新枚举类型：_referenceAttachmentProvider_ 和 _referenceAttachmentPermission_。 |

### <a name="change-notifications"></a>更改通知

| **更改类型** | **终结点** | **说明**                          |
| :-------------- | :----------- | :--------------------------------------- |
| 添加        | v1.0         | Webhook 现已在 v1.0 终结点上正式发布，可通过 _/Subscriptions_ 资源获取。 请创建、读取、续订和删除订阅，以接收 Outlook 和 Office 365 组对话数据的相关通知。 |

### <a name="users"></a>用户

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta 版本        | 添加了 mailboxSettings 属性和相应的类型。 |

## <a name="february-2016"></a>2016 年 2 月

### <a name="files"></a>文件

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 添加        | v1.0 和 beta | 在 Microsoft 帐户的 driveItem 上添加了新的 remoteItem 属性。 |

### <a name="general"></a>常规

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改          | v1.0 和 Beta | -/me/drive 现在同时适用于 Microsoft 帐户和工作及学校帐户。 |
| 更改          | v1.0 和 Beta | 对按需预配其 OneDrive 存储的帐户的驱动器请求工作更为可靠，且适用于租户默认的 SharePoint 网站使用非标准名称的更多场景。 |
| 删除        | Beta          | 删除了测试版架构中的各种未实现的类型，以便更加匹配 1.0 架构。 |

### <a name="change-notifications"></a>更改通知 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta 版本        | notificationUrl validation on subscription creation. For details, see [Microsoft Graph WebHooks Update - January 2016](https://developer.microsoft.com/office/blogs/Microsoft-Graph-WebHooks-Update-January-2016/). |
| 添加项        | Beta 版本        | 现在可删除订阅实体：DELETE https://graph.microsoft.com/beta/subscriptions/ |

### <a name="users"></a>用户

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 更改          | v1.0 和 Beta | 现在为 Microsoft 帐户返回 displayName。 |

## <a name="january-2016"></a>2016 年 1 月

### <a name="personal-contacts"></a>个人联系人 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | v1.0        | 向个人联系人实体集添加了 mobilePhone 属性。 |

### <a name="identity-and-access"></a>身份和访问 

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修补程序             | v1.0 和 beta | Fixed calling actions that are bound to directoryObjects, which were failing with the following error:  The return type from the operation is not possible with the given entity set. This applies to the following actions: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_. |

## <a name="december-2015"></a>2015 年 12 月

### <a name="personal-contacts"></a>个人联系人 

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 添加        | Beta 版本        | 向个人联系人实体集添加了 mobilePhone 属性。 |

### <a name="general"></a>常规

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修补程序             | v1.0 和 beta | 修复了使用 $filter 表达式多次指定同一属性，会出现以下 500 错误的请求：已添加具有相同键的项目。 |
| 修补程序             | v1.0 和 beta | 修复了对操作参数名称和值不区分大小写的错误。 |
| 修补程序             | v1.0 和 beta | 修复了对包含某些嵌入复杂属性的 null 值的有效负载的请求处理出现 null 引用异常的问题。 |
| 添加        | v1.0 和 beta | 添加了对复杂类型属性进行排序和筛选的支持。 |
| 添加项        | v1.0 和 beta | Added authorization_uri property in the www-authenticate header on a 401 response. This uri can be used to start the token acquisition flow. |
| 添加项        | v1.0 和 beta | 改进了用户和组中的错误消息。 |

### <a name="groups"></a>组

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修补程序             | v1.0 和 beta | 修复了无法调用以下组操作的问题：microsoft.graph.addFavorite、microsoft.graph.removeFavorite 和 microsoft.graph.resetUnseenCount。 |

### <a name="calendar"></a>日历

| **更改类型** | **Version** | **说明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Addition        | Beta        | 向 eventMessage 类型添加了 eventMessage 的 eventMessageRequest 子类型以及 startDateTime endDateTime、location、type、recurrence 和 isOutOfDate 属性。 |

### <a name="users"></a>用户

| **更改类型** | **Version**   | **说明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修补程序             | v1.0 和 beta | Fixed being able to select certain user properties on other users, when referencing the user by user principal name (UPN). For example: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| 修补程序             | v1.0 和 beta | 修复了在调用 _microsoft.graph.reminderView_ 用户绑定功能时出现以下错误的问题：无法在类型 Microsoft.OutlookServices.Reminder 上找到名为 businessPhones 的属性。 |
| 修补程序             | v1.0 和 beta | 修复了出现 400 错误的用户创建和更新 (POST/PATCH /v1.0/users)。 |

