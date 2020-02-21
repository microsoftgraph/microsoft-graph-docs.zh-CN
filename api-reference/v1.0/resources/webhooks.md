---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: aadd1cb451a5da1c8d546ce140bd8129ca9c2bf8
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162510"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>使用 Microsoft Graph API 获取更改通知

Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

| **资源** | **支持的资源路径** | **可包含在通知中的资源数据**                  |
|:----------------|:------------|:-----------------------------------------|
| Outlook [邮件][] | `/users/{id}/messages`<br>`/users/{id}/mailFolders('inbox')/messages` | 否 |
| Outlook [事件][] | `/users/{id}/events` | 否 |
| Outlook 个人[联系人][] | `/users/{id}/contacts` | 否 |
| [用户][] | `/users`（对所有用户更改）<br>`/users/{id}`（对特定用户更改） | 否 |
| [组][] | `/groups`（对所有组更改）<br>`/groups/{id}`（对特定组更改） | 否 |
| Office 365 组[对话][] | `groups/{id}/conversations` | 否 |
| 用户个人 OneDrive 上_任何_ [driveItem][] 文件夹层次结构内的内容 | `/me/drive/root` | 否 |
| OneDrive for Business 上 [driveItem][] _根文件夹_层次结构内的内容 | `/drives/{id}/root`<br> `/me/drive/root` | 否 |
| 安全[警报][] | `/security/alerts/{id}`（对特定警报更改） <br> `/security/alerts/?$filter`（对已筛选的警报更改） | 否 |
| Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta) | `/teams/allMessages`（所有团队中所有渠道中的消息）<br>`/teams/{id}/channels/{id}/messages`（特定频道中的消息）<br>`/chats/allMessages`（所有聊天中的消息）<br>`/chats/{id}/messages`（特定聊天中的消息） | 是 |

> **注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。

## <a name="permissions"></a>权限

通常订阅操作需要拥有对资源的读取权限。 例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。 [创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。 下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。

| 权限类型                        | 支持的资源类型                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委派 - 工作或学校帐户     | [警报][]、[联系人][]、[对话][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]|
| 委派 - 个人 Microsoft 帐户 | [联系人][]、[driveItem][]、[事件][]、[邮件][]                                        |
| 应用程序                            | [警报][]、[联系人][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]|


## <a name="see-also"></a>另请参阅

- [订阅资源类型](./subscription.md)
- [列出订阅](../api/subscription-list.md)
- [获取订阅](../api/subscription-get.md)
- [创建订阅](../api/subscription-post-subscriptions.md)
- [更新订阅](../api/subscription-update.md)
- [删除订阅](../api/subscription-delete.md)

[联系人]: ./contact.md
[对话]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[警报]: ./alert.md
