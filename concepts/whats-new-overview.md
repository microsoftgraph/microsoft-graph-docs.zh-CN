---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ea123de2fea1efdc4647238f6a953e21d49901db
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418208"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

你是否知道 Microsoft Graph 中的一些新功能来源于开发人员社区的热门请求？ 

Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 

在下面查看 Microsoft Graph 中新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 如需了解 API 更新的更多详情，请参阅 API 更改日志的 [9 月](changelog.md#september-2019)和 [8 月](changelog.md#august-2019)部分。 


## <a name="october-2019-new-and-generally-available"></a>2019 年 10 月：新版本和正式版

### <a name="mail"></a>邮件
使用新的 **message** 参数更新[回复](/graph/api/message-reply?view=graph-rest-1.0)邮件时任何可写的 [message](/graph/api/resources/message?view=graph-rest-1.0) 属性，例如 [将收件人添加到回复](/graph/api/message-reply#example ?view=graph-rest-1.0)。

### <a name="users"></a>用户
[获取](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0)或[设置](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0)[用户邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0)的用户首选日期和时间格式设置。 

## <a name="october-2019-new-in-preview"></a>2019 年 10 月：预览版中的新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在生产应用中使用它们。

### <a name="groups"></a>组
使用 **hideFromAddressLists** 和 **hideFromOutlookClients** 属性在 Outlook 用户界面的某些部分或 Outlook 客户端中控制[组](/graph/api/resources/group?view=graph-rest-beta)的可见性。

## <a name="september-2019-new-and-generally-available"></a>2019 年 9 月：新版本和正式版

### <a name="calendar-mail-and-group"></a>日历、邮件和组
[获取文件的原始内容或项目的 MIME 内容](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment)，该项目已作为[附件](/graph/api/resources/attachment?view=graph-rest-1.0)添加到[事件](/graph/api/resources/event?view=graph-rest-1.0)、[邮件](/graph/api/resources/message?view=graph-rest-1.0)或组[帖子](/graph/api/resources/post?view=graph-rest-1.0)。

### <a name="calendar-mail-outlook-task-personal-contact"></a>日历、邮件、Outlook 任务、个人联系人
使用 [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0) 函数在受支持的[格式](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values)之间转换 Outlook 项目 ID，包括 Microsoft Graph 默认 ID 格式和不可变的 ID 格式。 

以下资源支持 ID 格式转换：

- [附件](/graph/api/resources/attachment?view=graph-rest-1.0)
- [联系人](/graph/api/resources/contact?view=graph-rest-1.0)
- [事件](/graph/api/resources/event?view=graph-rest-1.0)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [邮件](/graph/api/resources/message?view=graph-rest-1.0)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0)

### <a name="mail"></a>邮件
[获取邮件的 MIME 内容](outlook-get-mime-message.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
使用 [Microsoft Graph 工具包](toolkit/overview.md)开发生产应用，该应用提供一致的 Microsoft 365 外观，可以节省从 Microsoft Graph 进行身份验证和访问数据的时间。

## <a name="september-2019-new-in-preview"></a>2019 年 9 月：预览版中的新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
Intune [9 月](changelog.md#september-2019)更新

### <a name="files"></a>文件
- 增强的同步支持：

  - 使用新的 **pendingOperations** 属性标识可能影响 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 的二进制内容的操作。
  - [还原](/graph/api/driveitem-restore?view=graph-rest-beta)已删除的 **driveItem**。 
- 使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file?view=graph-rest-beta)数据安全性和完整性。
- 获取或设置[照片](/graph/api/resources/photo?view=graph-rest-beta)的方向。 OneDrive 个人版上支持设置。

### <a name="identity-and-access"></a>标识和访问
- 使用新的 **identities** 属性并获取[用户](/graph/api/resources/user?view=graph-rest-beta)可用于登录帐户的标识。 这些标识可由组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 用于在租户的云应用程序中[同步标识](/graph/api/resources/synchronization-overview?view=graph-rest-beta)的增强功能：

  - 存储[同步作业](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)的设置
  - 指定对同步作业施加[隔离](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta)的原因

### <a name="teamwork"></a>团队合作
使用[团队](/graph/api/resources/team?view=graph-rest-beta)的**常规**频道或自定义[成员设置](/graph/api/resources/teammembersettings?view=graph-rest-beta)，让团队成员在**团队**中创建专用频道。

### <a name="users"></a>用户
- 获取或更新[用户](/graph/api/resources/user?view=graph-rest-beta)用于登录帐户的标识。 这些标识可由商业组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 获取或更新用户的[邮箱首选日期和时间格式设置](/graph/api/resources/mailboxsettings?view=graph-rest-beta)。


## <a name="want-to-stay-in-the-loop"></a>保持循环
- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [office 365 开发人员计划](https://developer.microsoft.com/zh-CN/office/dev-program)，免费订阅 Office 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/zh-CN/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

