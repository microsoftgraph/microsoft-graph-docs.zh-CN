---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 22deb547eda4301d1b8bb3f2830516aa2e3be682
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688638"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


## <a name="october-2021-new-and-generally-available"></a>2021 年 10 月：新增和正式版本

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
- [传输](/graph/api/call-transfer)活动对等呼叫。
- 将组呼叫传输给指定与会者（传输接收方）。

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
支持拨入电话访问和[联机会议](/graph/api/resources/onlinemeeting)（[音频会议](/graph/api/resources/audioConferencing)）使用多个收费和免费号码。

<!-- Hold off until permissions are deployed
As part of [privacy management in Microsoft 365](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true), subject rights request now debuts in both v1 and beta endpoints of Microsoft Graph. The [subject rights request API](/graph/api/resources/subjectrightsrequest) lets users make requests to review or manage their personal data in their organizations. It also lets organizations automate and scale managing these requests, helping them to meet industry regulations more efficiently.
-->

### <a name="education"></a>教育
支持[媒体](/graph/api/resources/educationMediaResource)文件或其他[外部常规资源](/graph/api/resources/educationExternalResource)作为[分配资源](/graph/api/resources/educationassignmentresource)。

### <a name="identity-and-access--applications"></a>标识和访问权限 | 应用程序
- 若要改进[应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)的许可体验，请指定[应用程序需要访问的资源](/graph/api/resources/requiredresourceaccess?view=graph-rest-beta&preserve-view=true)，包括应用程序所需的 OAuth 2.0 委派权限和应用程序角色集。
- 将所需 API 的数量限制为 50 个，将每个应用程序所需的权限限制为 400 个。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- 设置[设备](/graph/api/resources/device)的[扩展属性](/graph/api/resources/onpremisesextensionattributes)，并在[创建](/graph/api/device-post-devices)或[更新](/graph/api/device-update)设备时，在 Azure Active Directory 中管理这些属性。
- [代表登录的用户（设备所有者或相应的角色）获取 BitLocker 恢复密钥](/graph/api/bitlockerrecoverykey-get)。 获取恢复密钥会生成与最终用户体验存在奇偶校验的[审核日志](/azure/active-directory/reports-monitoring/concept-audit-logs)。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
通过 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) 的 **additionalNotificationRecipients** 属性，将清单中其他用户或组成员指定为接收访问评审进度的通知。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
将[条件访问策略](/graph/api/resources/conditionalaccesspolicy)中的设备指定为应用该策略时，负责管理的一部分[条件](/graph/api/resources/conditionalAccessConditionSet)。

### <a name="personal-contacts"></a>个人联系人
在个人 Microsoft 帐户中，对 [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-beta&preserve-view=true) 资源启用支持委派的权限（`Contacts.Read` 或 `Contacts.ReadWrite`）。

### <a name="teamwork"></a>Teamwork
- [通过[团队](/graph/api/resources/team)中的所有频道获取所有消息](/graph/api/channel-getallmessages)。
- 从用户参与的[所有聊天中获取所有消息](/graph/api/chats-getallmessages)，包括一对一聊天、群组聊天和会议聊天。
- 了解适用于 Microsoft Graph 中的 Microsoft Teams API 的[许可和付款模式](teams-licenses.md)。

### <a name="users"></a>用户
现在，Azure Active Directory (Azure AD) 服务的用户许可证，支持显示上次更新许可证分配[状态](/graph/api/resources/licenseassignmentstate)时的时间戳。 

## <a name="october-2021-new-in-preview-only"></a>2021 年 10 月：仅限预览版中的新增功能

### <a name="applications"></a>应用程序
使用[联合标识凭据](/graph/api/resources/federatedidentitycredential?view=graph-rest-beta&preserve-view=true)管理应用程序的凭据，并允许组织的云应用程序在不使用机密和证书的情况下访问 Azure AD。

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
使用 [participantInfo](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true) 资源类型的 **participantId** 属性，确定呼叫 [参与者](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true)。

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
启用[会议注册](/graph/api/resources/meetingregistration?view=graph-rest-beta&preserve-view=true)，并组织联机会议作为[网络研讨会](/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3)。 将会议与注册页关联，并选择将每个人或仅组织成员注册为[会议注册者](/graph/api/resources/meetingregistrant?view=graph-rest-beta&preserve-view=true)。 

### <a name="customer-booking"></a>客户预订
- 支持[预订服务](/graph/api/resources/bookingService?view=graph-rest-beta&preserve-view=true)的以下属性：
  - 启用向客户发送短信预约通知（**smsNotificationsEnabled** 属性）。
  - 客户可用于访问服务（**webUrl** 属性）的 URL。
- 通过以下其中一个或多个属性进行[预约](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true)：
  - 指定客户的时区（**customerTimeZone** 属性）。
  - 指定在线预约的 URL（**joinWebUrl** 属性）。
  - 启用向客户发送短信预约通知（**smsNotificationsEnabled** 属性）。
- 为[客户](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true)指定一个或多个地址和电话号码。
- 指定[员工成员](/graph/api/resources/bookingStaffMember?view=graph-rest-beta&preserve-view=true)所在的时区。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
[列出](/graph/api/virtualendpoint-list-serviceplans?view=graph-rest-beta&preserve-view=true)组织的云电脑订阅的 [Windows 365 服务计划](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true)。 在每个[服务计划类型](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true#cloudpcserviceplantype-values)（商业版或企业版）下，组织可以选择从按 vCPU、内存和存储等属性划分的多种计划配置中选择要订阅的计划。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
指定可[配置为对应用程序或服务主体的限制](/graph/api/resources/appmanagementconfiguration?view=graph-rest-beta&preserve-view=true)的[密钥凭据配置设置](/graph/api/resources/keycredentialconfiguration?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
启用以下其他[设置](/graph/api/resources/assignmentReviewSettings?view=graph-rest-beta&preserve-view=true)，查看[访问包分配策略](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)：
- 未在指定的有效时间内评审请求时的默认行为（**accessReviewTimeoutBehavior** 属性）。
- 向审阅者显示推荐（**isAccessRecommendationEnabled** 属性）。
- 要求审阅者提供审批理由（**isApprovalJustificationRequired** 属性）。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 指定[连续访问评估策略](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true)设置是应该迁移还是已迁移到[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)。
- 作为 Azure Active Directory [条件访问](/azure/active-directory/conditional-access/overview)的一部分，使用新的会议控制 [continuousAccessEvaluationSessionControl](/graph/api/resources/continuousAccessEvaluationSessionControl?view=graph-rest-beta&preserve-view=true) 来持续评估访问权限并制定访问权限决策。

### <a name="search--index"></a>搜索 | 索引
- 指定[外部连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)中内容的搜索体验的[设置](/graph/api/resources/externalconnectors-searchsettings?view=graph-rest-beta&preserve-view=true)。 例如，搜索结果的[显示模板](/graph/api/resources/externalconnectors-displaytemplate?view=graph-rest-beta&preserve-view=true)和用于选择显示模板的[规则](/graph/api/resources/externalconnectors-propertyRule?view=graph-rest-beta&preserve-view=true)。
- 将一个或多个[外部组](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-beta&preserve-view=true)关联到[外部连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)。 例如，外部组（如业务部门或工作组）可以确定对外部连接表示的数据源中内容的权限。
- 还可以在 **connectorId** 属性的 [外部连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)中指定 Teams 应用的 ID。

### <a name="users"></a>用户
当用户输入密码时，根据组织的密码验证策略实时[验证密码](/graph/api/user-validatePassword?view=graph-rest-beta&preserve-view=true)。 根据策略中的规则，[从验证获取详细信息](/graph/api/resources/passwordValidationInformation?view=graph-rest-beta&preserve-view=true)。


## <a name="september-2021-new-and-generally-available"></a>2021 年 9 月: 新增功能和正式发布

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
- 使用 [startHoldMusic](/graph/api/participant-startHoldMusic) 操作让 [参与者](/graph/api/resources/participant) 保持呼叫并在后台播放音乐。
- 使用 [stopHoldMusic](/graph/api/participant-stopHoldMusic) 操作重新合并之前呼叫保持的参与者。

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
- 获取 [Teams 直播](/microsoftteams/teams-live-events/what-are-teams-live-events)与会者报告的内容流。
- 获取或设置自动录制[联机会议](/graph/api/resources/onlineMeeting)的选项。
- 将 `OnlineMeetingArtifact.Read.All` 用为委派权限或应用程序权限，以读取联机会议的项目。 有关详细信息，请参阅 [联机会议权限](permissions-reference.md#online-meetings-permissions)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
云打印机状态包括 [Internet 打印协议 (IPP)](https://www.iana.org/assignments/ipp-registrations/ipp-registrations.xhtml) 中的所有标准值。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune v 1.0 版的每月更新。 在 [更改日志](https://developer.microsoft.com/graph/changelog)中，设置 2021 年 9 月的 **日期** 筛选器，并查找具有此相同标题的部分。

### <a name="files"></a>文件
- 通过 **恶意软件** 属性获取 [driveItem](/graph/api/resources/driveItem) 中检测到的病毒的详细信息。
- 使用 [delta](/graph/api/driveitem-delta) 函数不仅可以跟踪根文件夹的更改，还可以跟踪驱动器中其他文件夹的更改。

### <a name="identity-and-access--directory-management"></a>标识和访问权限 | 目录管理
基于角色的访问控制 (RBAC) 提供商可以在 Azure Active Director 中[管理角色](/graph/api/resources/rolemanagement)，方法是[定义可以在特定资源上执行的角色操作](/graph/api/resources/unifiedroledefinition)，基于这些角色定义为用户[分配角色](/graph/api/resources/unifiedroleassignment)，为他们授权相应的资源访问权限。

### <a name="search--query"></a>搜索 | 查询
- 聚合数值或字符串类型搜索结果，这些结果由 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview) 导入，并在 [架构](/graph/api/resources/schema) 中设置为可精简。请参阅有关 [使用聚合优化搜索结果](search-concept-aggregation.md) 的详细信息。
- 对任何可排序属性上的 OneDrive 和 SharePoint 搜索结果进行 [排序](/graph/api/resources/search-api-overview#sort-search-results)。 有关详细信息，请参阅 [使用 Microsoft 搜索 API 对搜索结果进行排序](search-concept-sort.md)。

### <a name="teamwork"></a>团队合作
使用一个操作 [provisionEmail](/graph/api/channel-provisionemail) 获取 [频道的电子邮件地址](/graph/api/resources/channel) (如果存在)，或者另创建一个。使用 [removeEmail](/graph/api/channel-removeemail) 操作删除电子邮件地址。

### <a name="workbooks-and-charts"></a>工作簿和图表
异步创建表行。 为了提高性能，创建多个表行的好做法是在 [create tableRow](/graph/api/table-post-rows) 操作中对其进行批处理并异步执行该操作。 遵循 [GET workbookOperation](/graph/api/workbookoperation-get) 操作和 [tableRowOperationResult](/graph/api/workbook-tableRowOperationResult) 函数，以获取新的 [workbookTableRow](/graph/api/resources/workbooktablerow) 资源。


## <a name="september-2021-new-in-preview-only"></a>2021 年 9 月: 仅预览版新增功能

### <a name="applications"></a>应用程序
使用安全断言标记语言 (SAML) 单点登录流可指定默认重定向 URI（[应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)的 **defaultRedirectUri** 属性），或确定将用户发送到的登录的具体重定向 URI（[webApplication](/graph/api/resources/webapplication?view=graph-rest-beta&preserve-view=true) 的 **redirectUriSettings** 属性）。 

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
获取 [联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) 的 [会议出席报告](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) 中的参与者总数。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
[创建用例](/graph/api/ediscovery-case-post?view=graph-rest-beta&preserve-view=true) 操作始终以大格式创建用例。 这扩大了用例大小限制，以容纳更高的数据总量和项目总数。 有关详细信息，请参阅 [大用例优势](/microsoft-365/compliance/advanced-ediscovery-large-cases?view=o365-worldwide&preserve-view=true#benefits-of-large-cases)。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- [将云电脑重新设置](/graph/api/manageddevice-reprovisioncloudpc?view=graph-rest-beta&preserve-view=true) 为已注册到 Intune 的云托管虚拟桌面。
- 使用新的虚拟 CPU (vCPU)和存储大小将云电脑升级或降级到其他配置，从而 [调整云电脑大小](/graph/api/manageddevice-resizecloudpc?view=graph-rest-beta&preserve-view=true)。
- [设置](/graph/api/virtualendpoint-post-onpremisesconnections?view=graph-rest-beta&preserve-view=true)、[列出](/graph/api/virtualendpoint-list-onpremisesconnections?view=graph-rest-beta&preserve-view=true)并对[本地网络连接](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true)[运行状况检查](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true)，以预配云电脑。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune beta 版每月更新。 在 [更改日志](https://developer.microsoft.com/graph/changelog)中，设置 2021 年 9 月的 **日期** 筛选器，并查找具有此相同标题的部分。

### <a name="education"></a>教育
- 允许教师为学生[重新分配](/graph/api/educationsubmission-reassign?view=graph-rest-beta&preserve-view=true)带有审阅反馈的作业[提交](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true)。
- 如果将 `Prefer: include-unknown-enum-members` 请求头应用于对 [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) 或 [educationAssignmentDefaults](/graph/api/resources/educationassignmentdefaults?view=graph-rest-beta&preserve-view=true) 资源执行操作，则支持仅向学生日历添加作业。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
[删除](/graph/api/accesspackageassignmentrequest-delete?view=graph-rest-beta&preserve-view=true)[accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) 以删除已拒绝或已完成的请求。

### <a name="identity-and-access--identity-and-sign-in"></a>标识和访问权限 | 标识和登录
- 允许用户使用 [软件 OATH 令牌](/graph/api/resources/softwareOathAuthenticationMethod?view=graph-rest-beta&preserve-view=true) 执行多重身份验证。 软件 OATH 令牌为基于软件的数字生成器，其使用 OATH 基于时间的一次性密码(TOTP)标准。
- 通过使用 [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true) 的 **numberMatchingRequiredState** 属性，确定根据 Azure AD 中策略的多重身份验证，是已启用还是已禁用数字匹配。
- 通过使用 [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true) 的 **displayAppInformationRequiredState** 属性，确定是否在其身份验证应用通知中显示用户其他上下文。
- 使用 [B2C](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true) 用户流程和[自助服务](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true)注册用户流程，以支持之前已弃用的[用户流程](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) API。

### <a name="security--attack-simulation-and-training"></a>安全 | 攻击模拟和训练
首次推出[攻击模拟和训练](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true) API，作为 [Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true) 中的可用服务。 该 API 使租户管理员能够列出启动的[模拟](/graph/api/attacksimulationroot-list-simulations?view=graph-rest-beta&preserve-view=true)练习和培训，并获取有关网络钓鱼模拟中用户在线行为的派生见解的[报告](/graph/api/resources/report-m365defender-reports-overview?view=graph-rest-beta&preserve-view=true)。

## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft 技术社区](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的初次发布。任何相关的 REST API 更新都在 Beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](https://developer.microsoft.com/graph/changelog/)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
