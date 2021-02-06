---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 3e98e857f4da494491b2e23b0ce971fd93c9765a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133215"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。


## <a name="february-2021-new-in-preview-only"></a>2021 年 2 月：仅预览版新增功能

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 在 [[访问包分配请求](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)，将地理位置信息分配给](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)。
- 获取所有可用访问包 [环境](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true) Sharepoint Online 资源存储地理位置的列表。

## <a name="january-2021-new-in-preview-only"></a>2021 年 1 月：仅限预览版新增功能

### <a name="cloud-communications"></a>云通信
- 以 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) 的形式组织实时事件 - 参见[示例](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token)。 
- 获取[与会者报告](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event)、[录制内容](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event)或实时事件的备选录制的内容流。
- 获取[外出](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true)用户的[状态](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true)，以及为该状态设置的任何消息。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- 为成功的[本地网络连接](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true)[更新 Active Directory 域密码](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true)。
- [在本地网络连接上运行运行状况检查](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true)现在可以在[本地连接运行状态检查](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true)资源中暴露 5 种其他错误类型。 有关错误类型的更多信息，请参阅 2021 年 1 月的[更改日志](https://developer.microsoft.com/graph/changelog)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
代表已登录用户在应用程序中使用委派权限：
- `PrinterShare.ReadBasic.All` 读取打印机共享的基本信息，不包括访问控制信息。
- `PrintConnector.Read.All` 读取打印连接器。
- `PrintConnector.ReadWrite.All` 读取或写入打印连接器。
- `PrintJob.Create` 创建打印作业并将内容上载到打印作业。
- `PrintSettings.Read.All` 读取租户范围的打印设置。
- `PrintSettings.ReadWrite.All` 读取或写入租户范围的打印设置。
- `Reports.Read.All` 读取每个指定用户或每个打印机的打印使用情况摘要。

### <a name="groups"></a>组
使用 **membershipRuleProcessingStatus** 属性获取基于规则的动态组的处理状态。 当用户的属性发生更改时，此选项非常有用，用户在基于规则的 [Microsoft 365 组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)中的会员资格将根据为组织设置的组会员资格规则重新评估。 

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 应用可以使用应用程序权限，让管理员管理用户的 [身份验证方法](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true)。
- 支持 [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) 作为用户登录或对 Azure AD 执行多因素身份验证的身份验证方法。
- 使用 [Microsoft Authenticator 策略](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true)可以定义配置设置以及启用 Microsoft Authenticator 作为身份验证方法的用户或组。 使用 Microsoft Authenticator 策略代替已弃用的 [Microsoft Authenticator 无密码手机登录策略](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true)。 
- 支持 [Windows Hello 企业版](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true)作为用户在不使用密码的情况下登录 Windows 设备的身份验证方法。

## <a name="december-2020-new-and-generally-available"></a>2020 年 12 月：新版本和正式版

### <a name="calendar"></a>日历
- 会议组织者可以使用 [事件](/graph/api/resources/event)的 **hideAttendees** 属性来控制与会者是否可以在会议“**跟踪**”列表中看到彼此。
- 组织者可用的 **isDraft** 属性和 [cancel](/graph/api/event-cancel) 方法的 GA，以及组织者和与会者可用的 [forward](/graph/api/event-forward) 方法的 GA，以更好地管理日历中的 [事件](/graph/api/resources/event)资源。
- [日历](/graph/api/resources/calendar) 的 **hexColor** 和 **isDefault** 属性的 GA 可以更好地管理日历。

### <a name="cloud-communications"></a>云通信
[状态](/graph/api/resources/presence)资源的 GA，允许获取一个或多个用户的状态信息，例如他们的可用性和用户活动。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
尝试新[教程](tutorial-riskdetection-api.md)，学习如何使用[身份保护 API ](/graph/api/resources/identityprotectionroot)来识别风险，并配置工作流以确认泄露或启用修复。

### <a name="teamwork"></a>团队合作
- [API 管理 Teams 应用安装](/graph/api/resources/teamsappinstallation) 的 GA，包括获取团队或用户个人范围内的 应用，或者添加、删除或更新该应用。
- [获取用户和 Teams 应用间的聊天](/graph/api/userscopeteamsappinstallation-get-chat)。

### <a name="use-the-toolkit"></a>使用工具包
Microsoft Graph 工具包 2.0 的 GA 版本 - 此版本包含新 [Microsoft Graph 待办任务组件](./toolkit/components/todo.md)（与 [Planner 任务组件](./toolkit/components/tasks.md)不同），以及增强的[个人卡片组件](./toolkit/components/person-card.md)。 更多信息请参阅[相关的博客文章](https://developer.microsoft.com/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/)。


## <a name="december-2020-new-in-preview-only"></a>2020 年 12 月：仅限预览版的新增功能

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
继续实现 [Microsoft 365 合规 API](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true) 的管道是[保管人](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true)资源及其相关操作和方法，以[释放](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true)或[激活](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true)保管人。 使用 **保管人** 资源可以访问 Exchange Online 邮箱、OneDrive for Business、SharePoint 网站 ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)) 和 Microsoft 365 组([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)) 中保管人的数据 ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true))。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
在 [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 资源的 **status** 属性中，将云管理虚拟机的故障状态统称为 `failed`。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [更新](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true)[打印作业](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true)的[配置](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true)。
- 有关重命名一些属性和重新键入关系的详细信息，请参阅 API 更改日志的 [2020 年 12 月](https://developer.microsoft.com/graph/changelog/)部分。

### <a name="education"></a>教育版
- 如果作业发布后添加了学生，教师可以通过使用 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) 资源的 **addedStudentAction** 属性来控制作业行为。
- 教师可以通过 **educationAssignment** 资源的 **notificationChannelUrl** 属性发布作业发布通知。

### <a name="identity-and-access"></a>身份和访问
获取或设置 Azure AD [使用条款](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true)[协议](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true)、[协议文件](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true)和 [agreementfilelocalization](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true) 的版本和创建元数据。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
作为 Azure Active Directory [权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true)的一部分，当希望访问组、应用程序或 SharePoint Online 网站的用户请求分配[访问包](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)时，他们现在可以响应[访问包分配请求](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)中[本地化内容](/graph/api/resources/accesspackagelocalizedcontent?view=graph-rest-beta&preserve-view=true)中表示的[问题](/graph/api/resources/accesspackagequestion?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 管理员可以将用户流与与外部用户共享的应用程序相关联，并在这些应用程序上启用[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)。 他们可以定制义自助注册用户流，并创建个性化的注册体验。 具体地说，它们建立[用于调用自定义用户流的注册启动事件的侦听器](/graph/api/resources/invokeuserflowlistener?view=graph-rest-beta&preserve-view=true)。 应用程序与用户流相关联后，进入该应用程序的用户将能够启动一个提供来宾帐户的注册流。
- 在 [Azure Active Directory 用户流](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true)或 [Azure Active Directory B2C 租户用户流](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true)中，可以管理语言默认值并[自定义在用户流中显示给用户的语言和字符串](/graph/api/resources/userflowlanguageconfiguration?view=graph-rest-beta&preserve-view=true)。
- 在用于 Azure AD 自助服务注册和 Azure AD B2C 注册的用户流中使用 [API 连接器](/graph/api/resources/identityapiconnector?view=graph-rest-beta&preserve-view=true)，以在特定步骤调用 API 以影响用户流的执行。
- 为租户定义[电子邮件 OTP 身份验证方法策略](/graph/api/resources/emailauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>团队合作
- 对于[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)、[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)或[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)环境中的[成员](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)资源，你现在可以：
  - 区分是 [Azure AD 用户](/graph/api/resources/aaduserconversationmember?view=graph-rest-beta&preserve-view=true)的成员，注意用户 ID、电子邮件地址和 Azure AD 租户 ID。 
  - [添加多个用户作为团队成员](/graph/api/conversationmembers-add?view=graph-rest-beta&preserve-view=true)。
- 对于[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)资源：
  - [获取指定用户参与的聊天中的所有消息](/graph/api/chats-getallmessages?view=graph-rest-beta&preserve-view=true)，包括一对一聊天、群聊和会议聊天。
  - 使用所有功能来列出、获取、添加、删除和更新聊天中的[应用程序](/graph/api/resources/teamsappinstallation?view=graph-rest-beta&preserve-view=true)或[选项卡](/graph/api/resources/teamstab?view=graph-rest-beta&preserve-view=true)。
  - 使用 **chatType** 属性可将一对一聊天与群聊或与联机会议关联的聊天区分开来。
  - [创建](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/chat-patch?view=graph-rest-beta&preserve-view=true)聊天。
  - 对于聊天上下文中的成员，请使用 **visibleHistoryStartDateTime** 属性设置或获取表示与该成员共享会话历史时间段的时间戳。
  - 在指定的聊天室中[创建](/graph/api/chat-post-members?view=graph-rest-beta&preserve-view=true)或[删除](/graph/api/chat-delete-members?view=graph-rest-beta&preserve-view=true)成员。 
- 对于[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)资源：
  - [通过团队中的所有频道获取所有消息](/graph/api/channels-getallmessages?view=graph-rest-beta&preserve-view=true)。
  - 团队所有者可以启用 [频道审核](/graph/api/resources/channelmoderationsettings?view=graph-rest-beta&preserve-view=true)，通过使用该频道的“**审核设置**”属性。以控制谁可以在该频道中发起新帖子或回复帖子。
- 作为 [Teams 应用程序定义](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true)的一部分，使用 **机器人** 关系连接到 [团队机器人](/graph/api/resources/teamworkbot?view=graph-rest-beta&preserve-view=true)。

### <a name="to-do-tasks"></a>待办任务
订阅[待办任务](/graph/api/resources/todoTask?view=graph-rest-beta&preserve-view=true)的[更改通知](webhooks.md)。

## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](https://developer.microsoft.com/graph/changelog/)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
