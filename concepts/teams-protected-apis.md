---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: f8c4fd35982d6fa36b49209255217989d121aac7
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516143"
---
# <a name="protected-apis-in-microsoft-teams"></a>Microsoft Teams 中的受保护 API

Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。 除了权限和许可之外，这些 API 还需要进行额外的验证，然后才能使用。


以下是当前受保护的 API：
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出频道消息](/graph/api/channel-list-messages)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道增量中的聊天消息](/graph/api/chatmessage-delta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道消息](/graph/api/chatmessage-get)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)[创建新频道消息订阅](/graph/api/subscription-post-subscriptions)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出消息回复](/graph/api/chatmessage-list-replies)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取消息回复](/graph/api/chatmessage-get)
* （使用不存在的[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)列出聊天，带或不带受保护的 API 权限）
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天中的消息](/graph/api/chat-list-messages)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天中的消息](/graph/api/chatmessage-get)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)[创建新聊天消息订阅](/graph/api/subscription-post-subscriptions)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出所有托管内容](/graph/api/chatmessage-list-hostedcontents)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取托管内容](/graph/api/chatmessagehostedcontent-get)

>[!NOTE]
>[发送消息](/graph/api/channel-post-messages) API 不受保护。

要请求访问这些受保护的 API，请填写下述[请求表单](https://forms.office.com/r/v3qjyzBCxD)。 我们通常每周三查看访问请求，并每星期五或星期一部署审批，除非在美国的主要假日周期间。这些周内的提交将在以下非假日周处理。 若要验证请求是否已获得批准，请于下一个适用的星期一测试应用程序访问权限。 如果我们对请求有其他问题，我们将与表单中指定的电子邮件联系。 

