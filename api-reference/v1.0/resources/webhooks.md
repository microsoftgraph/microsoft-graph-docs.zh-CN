---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。 客户端是配置其自己的 URL，以接收通知的 web 服务。 客户端应用程序使用通知更新时更改其状态。 有关详细信息，包括如何订阅和处理传入通知，请参阅 Set up 中用户数据的更改的通知。
ms.openlocfilehash: c7d468b7c5064911d27d3a93bc3160d03c2a4dc3
ms.sourcegitcommit: 02ead22efd4f10cd50f89c9f5aa3b6dfda96aeec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2018
ms.locfileid: "27123943"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>使用 Microsoft Graph API 获取更改通知

Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。 客户端是配置其自己的 URL，以接收通知的 web 服务。 客户端应用程序使用通知更新时更改其状态。 有关详细信息，包括如何订阅和处理传入通知，请参阅[设置通知用户数据中的更改](/graph/webhooks)。

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

- 邮件
- 事件
- 联系人
- 用户
- 组
- 组对话
- 在 OneDrive，包括与 SharePoint 网站关联的驱动器上共享的内容
- 用户的个人 OneDrive 文件夹
- 安全警报

## <a name="permissions"></a>Permissions

通常订阅操作需要拥有对资源的读取权限。例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。

| 权限类型                        | 支持的资源类型                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委派 - 工作或学校帐户     | [联系人][]、[对话][]、[驱动器][]、[事件][]、[组][]、[消息][]、[用户][]、[通知][] |
| 委派 - 个人 Microsoft 帐户 | [联系人][]、[驱动器][]、[事件][]、[消息][]                                        |
| 应用程序                            | [联系人][]、[对话][]、[驱动器][]、[事件][]、[组][]、[消息][]、[用户][]、[通知][] |

## <a name="see-also"></a>另请参阅

- [订阅资源类型](./subscription.md)
- [列表订阅](../api/subscription-list.md)
- [获取订阅](../api/subscription-get.md)
- [创建订阅](../api/subscription-post-subscriptions.md)
- [更新订阅](../api/subscription-update.md)
- [删除订阅](../api/subscription-delete.md)

[联系人]: ./contact.md
[对话]: ./conversation.md
[驱动器]: ./drive.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[通知]: ./alert.md