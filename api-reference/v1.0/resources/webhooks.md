---
title: 使用 Microsoft Graph API 获取更改通知
description: 为客户提供更改通知。
ms.localizationpriority: high
author: Jumaodhiss
ms.prod: change-notifications
doc_type: conceptualPageType
ms.openlocfilehash: 93c2b55d9515a2976716633d663dfdcb23a186b3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898942"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>使用 Microsoft Graph API 获取更改通知

命名空间：microsoft.graph

Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

| **资源** | **支持的资源路径** | **可包含在通知中的资源数据**                  |
|:----------------|:------------|:-----------------------------------------|
| 云打印 [打印机][] | 打印作业准备好下载时的变化（作业可打印事件）：<br>`/print/printers/{id}/jobs` | 不支持 |
| 云打印 [printTaskDefinition][] | 在队列中具有有效作业时的变化（作业启动事件）：<br>`/print/printtaskdefinition/{id}/tasks` | 否 |
| OneDrive（个人版）上的 [driveItem][] | 对 _任何文件夹_ 的层次结构内的内容更改：<br>`/users/{id}/drive/root` | 否 |
| OneDrive for Business 上的 [driveItem][] | 对 _根文件夹_ 的层次结构内的内容更改：<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | 否 |
| [组][] | 对所有组更改：<br>`/groups` <br>对特定组更改：<br>`/groups/{id}`<br>对特定组的所有者所做的更改：<br>`/groups/{id}/owners`<br>对特定组成员所做的更改：<br>`/groups/{id}/members`  | 否 |
| SharePoint [网站][]下的[列表][] | _列表_ 内的内容更改： <br>`/sites/{id}/lists/{id}` | 否 |
| Microsoft 365 组[对话][] | 查看组的对话：<br>`groups/{id}/conversations` | 否 |
| Outlook [邮件][] | 对用户邮箱中的所有邮件更改： <br>`/users/{id}/messages`<br>对用户收件箱中的所有邮件更改：<br>`/users/{id}/mailFolders('inbox')/messages` | 否 |
| Outlook [事件][] | 对用户邮箱中的所有事件更改：<br>`/users/{id}/events` | 否 |
| Outlook 个人[联系人][] | 对用户邮箱中的所有个人联系人更改：<br>`/users/{id}/contacts` | 否 |
| 安全[警报][] | 对特定警报更改：<br>`/security/alerts/{id}` <br>对已筛选的警报更改：<br> `/security/alerts/?$filter`| 否 |
| Teams [callRecord][] | 更改 _所有_ 呼叫记录： `/communications/callRecords` | 否 |
| Teams [聊天][] | 对租户中任何聊天的更改：<br>`/chats` <br>对特定聊天的更改：<br>`/chats/{id}` | 是 |
| Teams [chatMessage][] | 对所有团队中所有频道聊天消息更改：<br>`/teams/getAllMessages` <br>对特定频道中的聊天消息更改：<br>`/teams/{id}/channels/{id}/messages`<br>对所有聊天的消息更改：<br>`/chats/getAllMessages` <br>对特定聊天中的消息更改：<br>`/chats/{id}/messages` | 是 |
| Teams [频道][] | 对所有团队中频道的更改：<br>`/teams/getAllChannels` <br>对特定团队中频道的更改：<br>`/teams/{id}/channels` | 是 |
| Teams [conversationMember][] | 对特定团队中成员身份的更改：<br>`/teams/{id}/members` <br> 对特定团队下所有频道中的成员身份的更改：<br>`teams/{id}/channels/getAllMembers` <br> 对特定聊天中成员身份的更改：<br>`/chats/{id}/members` <br> 对所有聊天中成员身份的更改：<br>`/teams/getAllMembers` | 是 |
| Teams [团队][] | 对租户中任何团队的更改：<br>`/teams` <br>对特定团队的更改：<br>`/teams/{id}` | 是 |
| [待办事项任务][] | 对特定任务列表中的所有任务进行更改:<br>`/me/todo/lists/{todoTaskListId}/tasks`<br>对所有任务的更改:<br>`/me/todo/lists/alltasks` | 否 |
| [用户][] | 对所有用户更改：<br>`/users` <br>对特定用户更改：<br>`/users/{id}`| 否 |

> **注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。

## <a name="permissions"></a>权限

通常订阅操作需要拥有对资源的读取权限。 例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。 [创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。 下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。

| 权限类型                        | 支持的资源类型                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委派 - 工作或学校帐户     | [警报][], [频道][], [联系人][], [对话][], [conversationMember][], [driveItem][], [事件][], [组][], [列表][], [消息][], [团队][], [todoTask][], [用户][]|
| 委派 - 个人 Microsoft 帐户 | [联系人][], [driveItem][], [事件][], [列表][], [消息][], [todoTask][]                                        |
| Application                            | [警报][], [callRecord][], [频道][], [chatMessage][], [联系人][], [conversationMember][], [driveItem][], [事件][], [组][], [列表][], [消息][], [打印机][], [printTaskDefinition][], [团队][], [用户][]|


## <a name="see-also"></a>另请参阅

- [订阅资源类型](./subscription.md)
- [列出订阅](../api/subscription-list.md)
- [获取订阅](../api/subscription-get.md)
- [创建订阅](../api/subscription-post-subscriptions.md)
- [更新订阅](../api/subscription-update.md)
- [删除订阅](../api/subscription-delete.md)

[聊天]: ./chat.md
[chatMessage]: ./chatmessage.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversationMember]: ./conversationmember.md
[频道]: ./channel.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[callRecord]: ./callrecords-callrecord.md
[警报]: ./alert.md
[打印机]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[团队]: ./team.md
[待办事项任务]: ./todotask.md
[todoTask]: ./todotask.md

