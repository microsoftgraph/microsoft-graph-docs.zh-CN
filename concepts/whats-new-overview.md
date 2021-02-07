---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: dd2174e73bf03b0d78d8300a45e0248ab783f3fd
ms.sourcegitcommit: cee56ed143e73d1d47cb015b18e01c2808e760ab
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137802"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。


## <a name="february-2021-new-in-preview-only"></a>2021 年 2 月：仅预览版新增功能

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 在 [[访问包分配请求](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)，将地理位置信息分配给](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)。
- 获取所有可用访问包 [环境](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true) Sharepoint Online 资源存储地理位置的列表。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
在[SharePoint站点使用情况的详细报告](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true)中获取更多属性：anonymousLinkCount、companyLinkCount、externalSharing、地理位置、secureLinkForGuestCount、secureLinkForMemberCount、siteSensitivityLabelId 和 unmanagedDevicePolicy。

### <a name="use-sdks"></a>使用 SDK
请试用[Microsoft Graph Java SDK v3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)预览版！ 更多信息，请看相关[博客文章](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/)。

## <a name="january-2021-new-in-preview-only"></a>2021 年 1 月：仅限预览版新增功能

### <a name="cloud-communications"></a>云通信
- 以 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) 的形式组织实时事件 - 参见[示例](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token)。 
- 获取[与会者报告](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event)、[录制内容](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event)或实时事件的备选录制的内容流。
- 获取[外出](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true)用户的[状态](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true)，以及为该状态设置的任何消息。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- 为成功的[本地网络连接](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true)[更新 Active Directory 域密码](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true)。
- [在本地网络连接上运行运行状况检查](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true)现在可以在[本地连接运行状态检查](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true)资源中暴露 5 种其他错误类型。 有关错误类型的更多信息，请参阅 2021 年 1 月的[更改日志](https://developer.microsoft.com/graph/changelog)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [ 订阅更改云打印的通知](universal-print-webhook-notifications.md) - 当打印作业启动时，以及当打印机准备下载打印作业时。
- 获取[打印机](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true)状态的全部[可能值](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true#printerprocessingstatedetail-values)。
- 代表已登录用户在应用程序中使用委派权限：
  - `PrinterShare.ReadBasic.All` 读取打印机共享的基本信息，不包括访问控制信息。
  - `PrintConnector.Read.All` 读取打印连接器。
  - `PrintConnector.ReadWrite.All` 读取或写入打印连接器。
  - `PrintJob.Create` 创建打印作业并将内容上载到打印作业。
  - `PrintSettings.Read.All` 读取租户范围的打印设置。
  - `PrintSettings.ReadWrite.All` 读取或写入租户范围的打印设置。
  - `Reports.Read.All` 读取每个指定用户或每个打印机的打印使用情况摘要。

### <a name="education"></a>教育版
使用班级[作业设置](/graph/api/resources/educationAssignmentSettings?view=graph-rest-beta&preserve-view=true)来启用或禁用动画来以庆祝交作业。

### <a name="groups"></a>组
使用 **membershipRuleProcessingStatus** 属性获取基于规则的动态组的处理状态。 当用户的属性发生更改时，此选项非常有用，用户在基于规则的 [Microsoft 365 组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)中的会员资格将根据为组织设置的组会员资格规则重新评估。 

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
获取用户或设备对构建在PowerApps上的第三方软件的[使用权](/graph/api/resources/UsageRight?view=graph-rest-beta&preserve-view=true)，或者，设备对订阅的使用权。 使用权包括相应服务或产品的标识符，以及使用权的当前状态，如激活、未激活、警告或暂停。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 应用可以使用应用程序权限，让管理员管理用户的 [身份验证方法](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true)。
- 支持 [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) 作为用户登录或对 Azure AD 执行多因素身份验证的身份验证方法。
- 使用 [Microsoft Authenticator 策略](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true)可以定义配置设置以及启用 Microsoft Authenticator 作为身份验证方法的用户或组。 使用 Microsoft Authenticator 策略代替已弃用的 [Microsoft Authenticator 无密码手机登录策略](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true)。 
- 支持 [Windows Hello 企业版](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true)作为用户在不使用密码的情况下登录 Windows 设备的身份验证方法。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
- [获取注册用户数的报告，或能够使用各种注册功能的用户数](/graph/api/authenticationmethodsroot-usersregisteredbyfeature?view=graph-rest-beta&preserve-view=true)，包括多因素认证、自助密码重置或无密码认证。
- [获取每种认证方式的注册用户数报告](/graph/api/authenticationmethodsroot-usersregisteredbymethod?view=graph-rest-beta&preserve-view=true)，包括密码、Windows Hello 企业版或无密码电话登录。

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
