---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: e14227ad1e64aaea6bf2cfb15f9ba76d0ffeb12b
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219648"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>使用 Microsoft Graph API 获取更改通知

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

| **资源** | **支持的资源路径** | **资源数据可以包含在通知中**                  |
|:----------------|:------------|:-----------------------------------------|
| Outlook [邮件][] | 对用户邮箱中的所有邮件所做的更改： <br>`/users/{id}/messages`<br>对用户收件箱中的邮件所做的更改：<br>`/users/{id}/mailFolders('inbox')/messages` | 否 |
| Outlook [事件][] | 对用户邮箱中的所有事件所做的更改：<br>`/users/{id}/events` | 否 |
| Outlook 个人[联系人][] | 对用户邮箱中的所有个人联系人所做的更改：<br>`/users/{id}/contacts` | 否 |
| [用户][] | 对所有用户所做的更改：<br>`/users` <br>对特定用户的更改：<br>`/users/{id}`| 否 |
| [组][] | 对所有组所做的更改：<br>`/groups` <br>对特定组的更改：<br>`/groups/{id}` | 否 |
| Office 365 组[对话][] | 对组的对话所做的更改：<br>`groups/{id}/conversations` | 否 |
| OneDrive （个人版）上的[driveItem][] | 对_任意文件夹_层次结构中的内容所做的更改：<br>`/users/{id}/drive/root` | 否 |
| OneDrive for Business 上的[driveItem][] | 对_根文件夹_层次结构中的内容所做的更改：<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | 否 |
| 安全[警报][] | 对特定警报的更改：<br>`/security/alerts/{id}` <br>对已筛选警报的更改：<br> `/security/alerts/?$filter`| 否 |
| 团队[了 chatmessage](/graph/api/resources/subscription?view=graph-rest-beta) | 对所有团队中的所有频道中的聊天消息的更改：<br>`/teams/allMessages` <br>对特定频道中聊天邮件的更改：<br>`/teams/{id}/channels/{id}/messages`<br>在所有聊天中对聊天消息进行的更改：<br>`/chats/allMessages` <br>在特定聊天中对聊天消息进行的更改：<br>`/chats/{id}/messages` | 是 |

> **注意**：开头的`/users/{id}`任何资源路径也都可以接受`/me`引用已登录用户。

## <a name="permissions"></a>权限

通常订阅操作需要拥有对资源的读取权限。 例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。 [创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。 下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。

| 权限类型                        | 支持的资源类型                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委派 - 工作或学校帐户     | [警报][]、[联系人][]、[对话][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]|
| 委派 - 个人 Microsoft 帐户 | [联系人][]、[driveItem][]、[事件][]、[邮件][]                                        |
| 应用程序                            | [alert][]、 [contact][]、 [driveItem][]、 [event][]、 [group][]、 [message][]、 [user][]、[了 chatmessage][]|

## <a name="see-also"></a>另请参阅

- [订阅资源类型](subscription.md)
- [列出订阅](../api/subscription-list.md)
- [获取订阅](../api/subscription-get.md)
- [创建订阅](../api/subscription-post-subscriptions.md)
- [更新订阅](../api/subscription-update.md)
- [删除订阅](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
[contact]: ./contact.md
[对话]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[警报]: ./alert.md
