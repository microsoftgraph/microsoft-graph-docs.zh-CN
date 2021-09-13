---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: ea31eafc933f0ec83cfbb00ecc652812223d9516
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083829"
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

要请求访问这些受保护的 API，请填写下述[请求表单](https://aka.ms/teamsgraph/requestaccess)。 我们在每周三审查访问请求，并在每周五部署批准，但美国的主要节假日周除外。在这些周中的提交将在下一个非节假日周进行处理。

如果除了表单，还想要提供其他信息，可与 [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) 联系。
请在所有通信中包含应用 ID。
