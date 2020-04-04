---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: d8f8c8450f568917e5211048c164e02ad503e869
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108191"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>使用 Microsoft Graph API 获取更改通知

命名空间：microsoft.graph

Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

| **资源** | **支持的资源路径** | **可包含在通知中的资源数据**                  |
|:----------------|:------------|:-----------------------------------------|
| Outlook [邮件][] | 对用户邮箱中的所有邮件更改： <br>`/users/{id}/messages`<br>对用户收件箱中的所有邮件更改：<br>`/users/{id}/mailFolders('inbox')/messages` | 否 |
| Outlook [事件][] | 对用户邮箱中的所有事件更改：<br>`/users/{id}/events` | 否 |
| Outlook 个人[联系人][] | 对用户邮箱中的所有个人联系人更改：<br>`/users/{id}/contacts` | 否 |
| [用户][] | 对所有用户更改：<br>`/users` <br>对特定用户更改：<br>`/users/{id}`| 否 |
| [组][] | 对所有组更改：<br>`/groups` <br>对特定组更改：<br>`/groups/{id}` | 否 |
| Office 365 组[对话][] | 查看组的对话：<br>`groups/{id}/conversations` | 否 |
| OneDrive（个人版）上的 [driveItem][] | 对_任何文件夹_的层次结构内的内容更改：<br>`/users/{id}/drive/root` | 否 |
| OneDrive for Business 上的 [driveItem][] | 对_根文件夹_的层次结构内的内容更改：<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | 否 |
| SharePoint [网站][]下的[列表][] | _列表_内的内容更改： <br>`/sites/{id}/lists/{id}` | 否 |
| 安全[警报][] | 对特定警报更改：<br>`/security/alerts/{id}` <br>对已筛选的警报更改：<br> `/security/alerts/?$filter`| 否 |
| Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-v1.0) | 对所有团队中所有频道聊天消息更改：<br>`/teams/allMessages` <br>对特定频道中的聊天消息更改：<br>`/teams/{id}/channels/{id}/messages`<br>对所有聊天的消息更改：<br>`/chats/allMessages` <br>对特定聊天中的消息更改：<br>`/chats/{id}/messages` | 是 |

> **注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。

## <a name="permissions"></a>权限

通常订阅操作需要拥有对资源的读取权限。 例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。 [创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。 下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。

| 权限类型                        | 支持的资源类型                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委派 - 工作或学校帐户     | [警报][]、[联系人][]、[对话][]、[driveItem][]、[列表][]、 [事件][]、[组][]、[邮件][]、[用户][]|
| 委派 - 个人 Microsoft 帐户 | [联系人][]、[driveItem][]、[列表][]、[事件][]、[邮件][]                                        |
| 应用程序                            | [警报][]、[联系人][]、[列表][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]|


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
[list]: ./list.md
[site]: ./site.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[警报]: ./alert.md
