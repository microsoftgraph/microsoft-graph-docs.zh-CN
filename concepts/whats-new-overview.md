---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: f4ea5833922cbc36465bba32a7f4ade9b18c11d8
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629004"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


## <a name="may-2022-new-and-generally-available"></a>2022 年 5 月：新版本和正式版

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
在 Azure Active Directory (Azure AD) 中注册的[应用程序](/graph/api/resources/application)可以指定服务或资产管理数据库中的应用程序或服务联系人信息。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
允许 Azure Active Directory (Azure AD)租户设置 [与另一个标识提供程序(IdP)支持 SAML 或 WS-Fed 协议的组织联盟](/graph/api/resources/samlOrWsFedExternalDomainFederation)。 这使得 Azure AD 租户能够允许来宾用户访问其资源。

### <a name="sites-and-lists"></a>网站和列表
- 通过使用 [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes)操作，从内容类型中心获取兼容的 [内容类型](/graph/api/resources/contentType) 资源集合。 
- 使用 [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub) 操作，将内容类型从内容类型中心添加或同步到 [网站](/graph/api/resources/site) 或 [列表](/graph/api/resources/list)。 这使得内容类型或其更新可用于需要它的特定站点或列表。 这是对传统同步基础结构的一项改进，后者将内容类型推送到整个组织中的所有站点，从而减少了发布传播的等待时间。 
- 获取一个或多个在站点或列表上发生的[丰富的长时间运行的操作](/graph/api/resources/richlongrunningoperation)，在同步添加内容类型时可能会发生这种情况。

### <a name="teamwork"></a>Teamwork
[获取频道上的消息](/graph/api/channel-list-messages)，并包含对消息 [的任何答复](/graph/api/channel-list-messages#example-3-request-with-top-and-expand-query-options-on-replies)。


## <a name="may-2022-new-in-preview-only"></a>2022 年 5 月：仅限预览版中的新增功能

### <a name="application"></a>应用程序
为本地应用程序配置 Azure AD 应用程序代理以实现安全的远程访问时，请使用 [onPremisesPublishing](/graph/api/resources/onPremisesPublishing?view=graph-rest-beta&preserve-view=true) 资源中的 **isStateSessionEnabled** 属性，指定如果应用程序使用 OAuth 2.0 授权代码授予流，是否验证状态参数。 设置此属性有助于管理员保护应用，以避免出现跨网站请求伪造 (CSRF) 。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
[授权策略](/graph/api/resources/authorizationPolicy?view=graph-rest-beta&preserve-view=true)的[默认用户角色](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true)可以指定设备的注册所有者是否可以读取自己的 BitLocker 恢复密钥。

### <a name="search--index"></a>搜索 | 索引
[获取](/graph/api/externalconnectors-connectionquota-get?view=graph-rest-beta&preserve-view=true)[连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)的[配额信息](/graph/api/resources/externalconnectors-connectionQuota?view=graph-rest-beta&preserve-view=true)。 此信息包括可以引入到连接中的项数，并包括连接中剩余的项目，及其所有连接的租户级剩余配额。



## <a name="april-2022-new-and-generally-available"></a>2022 年 4 月：新版本和正式版

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
在生产应用中使用[特权标识管理 (PIM)](/graph/api/resources/privilegedidentitymanagementv3-overview)管理、控制和监视对组织中重要资源的访问。 通过特权角色和基于角色的访问控制 (RBAC) 启用访问权限，并且可以向用户、组或服务主体授予权限。 资源可以位于 Azure AD、Azure 和其他 Microsoft 云服务中，例如 Microsoft 365 或 Microsoft Intune。

### <a name="search--index"></a>搜索 | 索引
- 使用应用程序权限 `ExternalConnection.Read.All` 和 `ExternalConnection.ReadWrite.All` 在没有登录用户的情况下读取或写入所有外部连接。
- 使用应用程序权限 `ExternalItem.Read.All` 在没有登录用户的情况下读取所有外部项。
- 使用委托的权限 `ExternalConnection.ReadWrite.OwnedBy` 代表已登录用户读取和写入外部连接，应用已获授权。
- 使用委托的权限 `ExternalConnection.Read.All` 或 `ExternalConnection.ReadWrite.All` 代表已登录用户读取或写入所有外部连接。
- 使用委托的权限 `ExternalItem.ReadWrite.OwnedBy` 代表已登录的用户读取和写入外部项，应用已获授权。
- 使用委托的权限 `ExternalItem.Read.All` 或 `ExternalItem.ReadWrite.All` 代表已登录用户读取或写入所有外部项。


## <a name="april-2022-new-in-preview-only"></a>2022 年 4 月：仅限预览版中的新增功能

### <a name="customer-bookings"></a>客户预订
- [获取[企业](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true)中[员工成员](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true)资源的可用信息](/graph/api/bookingbusiness-getstaffavailability?view=graph-rest-beta&preserve-view=true)。
- 使用面向`Bookings.Read.All`[企业](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true)、[员工成员](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true)、[服务](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true)、[客户](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true)和[预约](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true)资源的读取操作中的应用程序权限。
- 对客户和预约资源使用读/写操作的应用程序权限 `BookingsAppointment.ReadWrite.All`。

### <a name="device-and-app-management--cloud-pc"></a>设备和应用管理|云电脑
- 将 [Windows 设置](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true)指定为租户的[云电脑组织设置](/graph/api/resources/cloudPcOrganizationSettings?view=graph-rest-beta&preserve-view=true)的一部分。
- [获取](/graph/api/user-list-cloudpcs?view=graph-rest-beta&preserve-view=true)归属于已登录用户的云电脑设备。
- [获取信息以为已登录用户启动云电脑设备](/graph/api/cloudpc-getcloudpclaunchinfo?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
配置[联合身份验证设置](/graph/api/resources/internalDomainFederation?view=graph-rest-beta&preserve-view=true)，将域与 Azure Active Directory 联合。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
[获取](/graph/api/accesspackageassignment-additionalaccess?view=graph-rest-beta&preserve-view=true) 相应用户具有不兼容的访问包的分配。 

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
通过在相应的 Azure Active Directory 登录日志中标记事件，确认事件存在[高风险且已泄露](/graph/api/signin-confirmCompromised?view=graph-rest-beta&preserve-view=true)或[安全](/graph/api/signin-confirmSafe?view=graph-rest-beta&preserve-view=true)。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
- 获取指定时间段内特定 Teams 活动的计数的[总分布报告](/graph/api/reportroot-getTeamsUserActivityTotalDistributionCounts?view=graph-rest-beta&preserve-view=true)。 Teams 活动的计数包括团队聊天消息、通话、会议、音频持续时间、发布消息等。
- 在报告中获取其获取用户详细信息，包括[获取用户详细信息](/graph/api/reportroot-getTeamsUserActivityUserDetail?view=graph-rest-beta&preserve-view=true)、[获取活动计数](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta&preserve-view=true)，以及[获取活动总计数](/graph/api/reportroot-getteamsuseractivitytotalcounts?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>Teamwork
与一个或多个团队共享频道：
- [仅列出与团队共享的频道](/graph/api/team-list-incomingchannels?view=graph-rest-beta&preserve-view=true)。
- [列出团队中的所有频道](/graph/api/team-list-allchannels?view=graph-rest-beta&preserve-view=true)，包括在团队中托管或与团队共享的频道。
- [列出可以访问指定共享通道的团队成员](/graph/api/sharedwithchannelteaminfo-list-allowedmembers?view=graph-rest-beta&preserve-view=true)。
- [删除与团队共享的频道](/graph/api/team-delete-incomingchannel?view=graph-rest-beta&preserve-view=true)。
- [列出已共享指定频道的团队](/graph/api/sharedwithchannelteaminfo-list?view=graph-rest-beta&preserve-view=true)。
- [取消与团队共享频道](/graph/api/sharedwithchannelteaminfo-delete?view=graph-rest-beta&preserve-view=true)。


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
