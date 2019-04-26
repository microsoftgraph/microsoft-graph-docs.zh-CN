---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 webhook 机制将更改通知传递给客户端。 客户端是用于配置自身的 URL 以接收通知的 Web 服务。 客户端应用使用通知在更改时更新其状态。 有关更多详细信息, 包括如何订阅和处理传入通知, 请参阅设置用户数据中的更改通知。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 8422328061ac1c2ad736435204b699544bffd2ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341503"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>使用 Microsoft Graph API 获取更改通知

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph REST API 使用 webhook 机制将更改通知传递给客户端。 客户端是用于配置自身的 URL 以接收通知的 Web 服务。 客户端应用使用通知在更改时更新其状态。 有关更多详细信息, 包括如何订阅和处理传入通知, 请参阅[设置用户数据中的更改通知](/graph/webhooks)。

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

- Outlook [邮件][]
- Outlook [事件][]
- Outlook 个人[联系人][]
- [用户][]
- [组][]
- Office 365 组[对话][]
- 用户个人 OneDrive 上_任何_ [driveItem][] 文件夹层次结构内的内容
- OneDrive for Business 上 [driveItem][] _根文件夹_层次结构内的内容
- 安全[警报][]

## <a name="permissions"></a>权限

通常情况下, 订阅操作需要对资源具有读取权限。 例如, 若要获取邮件的通知, 您的应用程序`Mail.Read`需要该权限。 [创建订阅](../api/subscription-post-subscriptions.md)文章列出了每种资源类型所需的权限。 下表列出了您的应用程序可以请求对特定资源类型使用 webhook 的权限类型。

| 权限类型                        | 支持的资源类型                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委派的工作或学校帐户     | [警报][]、[联系人][]、[对话][]、 [driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]|
| 委派-个人 Microsoft 帐户 | [contact][]、 [driveItem][]、 [event][]、 [message][]                                        |
| 应用程序                            | [alert][]、 [contact][]、 [driveItem][]、 [event][]、 [group][]、 [message][]、 [user][]|

## <a name="see-also"></a>另请参阅

- [订阅资源类型](subscription.md)
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
