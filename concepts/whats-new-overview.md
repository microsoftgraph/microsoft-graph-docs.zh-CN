---
title: Microsoft Graph 新增功能
description: 查看过去两个月 Microsoft Graph 中的新增功能、早期版本中添加的内容以及如何分享你的想法的亮点。
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 26b4024a3fd23fb2ea9f2ee04a02894b16db6e0d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735332"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。

## <a name="july-2022-new-in-preview-only"></a>2022 年 7 月：仅限预览版中的新增功能

### <a name="cloud-communications--call"></a>云通信 | 呼叫
使用加入会议 ID 或密码 [加入计划通话](/graph/api/application-post-calls?view=graph-rest-beta&preserve-view=true)。

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
[创建](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-4-create-an-online-meeting-that-requires-a-passcode) 需要密码的 [联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)。

### <a name="users"></a>用户
[获取](/graph/api/user-get?view=graph-rest-beta&preserve-view=true) Windows 方案中用户的安全标识符 (SID)。

## <a name="june-2022-new-and-generally-available"></a>2022 年 6 月：新版本和正式发布版本

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
在 [获取呼叫记录](/graph/api/callrecords-callrecord-get) 并展开 [会话](/graph/api/resources/callrecords-session) 的每个 [区段](/graph/api/resources/callrecords-segment) 时，获取有关 [媒体流](/graph/api/resources/callrecords-mediastream) 的音频编解码器、视频编解码器、网络传输协议和跟踪路由跃点的信息。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- [列出管理单元](/graph/api/device-list-memberOf)（[设备](/graph/api/resources/device)所属）。
- 将设备作为 [管理单元](/graph/api/resources/administrativeunit) 中的成员进行管理：[列出成员](/graph/api/administrativeunit-list-members)（包括设备），并 [获取](/graph/api/administrativeunit-get-members)、[添加](/graph/api/administrativeunit-post-members) 和 [删除](/graph/api/administrativeunit-delete-members) 作为成员的设备。 
- [获取](/graph/api/application-get) 应用程序 [的安全性和符合性认证](/graph/api/resources/certification) 的状态和其他详细 [信息，以保护](/graph/api/resources/application) 客户数据。 有关详细信息，请 [参阅Microsoft 365认证](/microsoft-365-app-certification/docs/enterprise-app-certification-guide)。
- 使用 [Azure AD配置联合设置](/graph/api/resources/internalDomainFederation)。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 配置和管理租户中 [临时访问通行证身份验证方法策略的设置](/graph/api/resources/temporaryAccessPassAuthenticationMethodConfiguration)。
- 获取[目录中用于跨租户访问设置的基本策略](/graph/api/resources/crosstenantaccesspolicy)，关于组织如何与外部 Azure Active Directory 组织交互的[默认配置](/graph/api/resources/crosstenantaccesspolicyconfigurationdefault)，以及外部 Azure Active Directory 组织的[特定于合作伙伴的配置](/graph/api/resources/crosstenantaccesspolicyconfigurationpartner)。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
在由以下方法生成的 Teams 报表中查找新列：
  - [getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts)
  - [getTeamsUserActivityUserDetail](/graph/api/reportroot-getTeamsUserActivityUserDetail)
  - [getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getTeamsDeviceUsageUserDetail)
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)
- 已弃用以下方法生成的 Teams 报表中的 Windows Phone 列：
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)

### <a name="teamwork"></a>Teamwork
在 Teams 中订阅以下内容的更改通知：
- [团队和频道](teams-changenotifications-team-and-channel.md)
- [团队和频道成员身份](teams-changenotifications-teammembership.md)
- [聊天](teams-changenotifications-chat.md)
- [聊天成员身份](teams-changenotifications-chatmembership.md)
- [所有特定用户所属的聊天中的聊天消息](/graph/teams-changenotifications-chatmessage#subscribe-to-changes-at-the-user-level)。

## <a name="june-2022-new-in-preview-only"></a>2022 年 6 月：新增功能（仅限预览版）

### <a name="applications"></a>应用程序
指定[链接对象](/graph/api/resources/synchronization-synchronizationLinkedObjects?view=graph-rest-beta&preserve-view=true)，这些对象可以[在按需预配期间预配](/graph/api/resources/synchronization-synchronizationJobSubject?view=graph-rest-beta&preserve-view=true)，包括经理、成员、所有者等主体。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
从 [安全](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true) 命名空间（而不是符合性命名空间）访问 [电子数据展示 API](/graph/api/resources/security-ediscoverycase?view=graph-rest-beta&preserve-view=true)。

### <a name="compliance--records-management"></a>合规性｜记录管理
使用首次 [Microsoft Purview 记录管理 API](/graph/api/resources/security-recordsmanagement-overview?view=graph-rest-beta&preserve-view=true) 帮助组织管理数据的保留和删除，以满足法律义务和合规性法规。

### <a name="customer-booking"></a>客户预订
- 管理 [企业或企业](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true) 提供的 [服务](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true) 自助预订页面的语言。
- 在 [客户信息](/graph/api/resources/bookingCustomerInformation?view=graph-rest-beta&preserve-view=true) 中指定是否为客户的 [约会](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true) 启用短信通知。
- 指定是否为 [服务](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true)启用匿名联接，以及是否为服务的约会生成匿名联接 Web URL。
- 区分 [员工成员](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) 作为计划程序或成员的角色。
- 指定在为 [该成员](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) 分配预订或更新预订时是否通过电子邮件通知员工成员。

### <a name="device-and-app-management--cloud-pc"></a>设备和应用管理|云电脑
获取云电脑 [预配](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true)策略的以下信息：
- 云电脑所在的组的名称。
- 在重新预配/取消预配之前等待的小时数。
- 是否启用本地管理员（例如云电脑的最终用户）。
- 管理 Azure 网络连接的服务，当前为 Windows 365 或 Microsoft Dev Box。

### <a name="device-and-app-management--multi-tenant-management"></a>设备和应用管理|多租户管理
[获取](/graph/api/managedtenants-managedtenant-list-myroles?view=graph-rest-beta&preserve-view=true) [分配给已登录到](/graph/api/resources/managedtenants-myRole?view=graph-rest-beta&preserve-view=true) 托 [管租户](/graph/api/resources/managedtenants-managedTenant?view=graph-rest-beta&preserve-view=true)的用户的角色的集合。

### <a name="education"></a>教育
- 为 [分配](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) [创建](/graph/api/educationassignment-setupfeedbackresourcesfolder?view=graph-rest-beta&preserve-view=true) SharePoint 文件夹，以上传反馈文档。
- 在与分配关联的反馈文件夹中 [创建](/graph/api/educationfeedbackresourceoutcome-post-outcomes?view=graph-rest-beta&preserve-view=true) [提交](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) 的 [反馈文档](/graph/api/resources/educationFeedbackResourceOutcome?view=graph-rest-beta&preserve-view=true)。

### <a name="groups"></a>组
指定是否将[组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)[配置为将组对象属性写回](/graph/api/resources/groupWritebackConfiguration?view=graph-rest-beta&preserve-view=true)本地 Active Directory。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- 将已验证的子域 [升级](/graph/api/domain-promote?view=graph-rest-beta&preserve-view=true) 为根域。
- [获取](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) [单租户应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)联合的 SAML 元数据的 URL。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
隐藏租户登录页的 [登录页文本可见性设置](/graph/api/resources/loginpagetextvisibilitysettings?view=graph-rest-beta&preserve-view=true) 中的自助式密码重置 (SSPR) 链接。

### <a name="teamwork"></a>团队合作
- 获取在[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)或 [频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) 中 [固定](/graph/api/resources/messagePinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) 或 [取消固定](/graph/api/resources/messageUnpinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) 的详细信息。 
- 作为支持导出 Teams 内容的方案，你可以 [列出](/graph/api/teamwork-list-deletedteams?view=graph-rest-beta&preserve-view=true) 已删除的团队，并 [获取](/graph/api/deletedteam-getallmessages?view=graph-rest-beta&preserve-view=true) 某个 [已删除团队](/graph/api/resources/deletedTeam?view=graph-rest-beta&preserve-view=true) 的 1:1 聊天、群组聊天、会议聊天和频道消息。 有关详细信息，请参阅 [使用 Microsoft Teams 导出 API 导出内容](/microsoftteams/export-teams-content)。


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft 反馈门户](https://aka.ms/graphfeedback) 提出有关新功能的建议并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [加入](https://aka.ms/m365-dev-call) 每周Microsoft 365平台社区通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](https://developer.microsoft.com/graph/changelog/)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
