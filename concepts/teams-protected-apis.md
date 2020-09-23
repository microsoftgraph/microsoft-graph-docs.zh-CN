---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8838c7981d82b6b9096ba4c6c13b5d6350b45ab4
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223420"
---
# <a name="protected-apis-in-microsoft-teams"></a>Microsoft Teams 中的受保护 API

Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。 除了权限和许可之外，这些 API 还需要进行额外的验证，然后才能使用。

以下是当前受保护的 API：
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出频道消息](/graph/api/channel-list-messages)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道增量中的聊天消息](/graph/api/chatmessage-delta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道消息](/graph/api/channel-get-message)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)[创建新频道消息订阅](/graph/api/subscription-post-subscriptions)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出消息回复](/graph/api/channel-list-messagereplies)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取消息回复](/graph/api/channel-get-messagereply)
* （使用不存在的[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)列出聊天，带或不带受保护的 API 权限）
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天中的消息](/graph/api/chat-list-message)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天中的消息](/graph/api/chat-get-message)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)[创建新聊天消息订阅](/graph/api/subscription-post-subscriptions)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出所有托管内容](/graph/api/chatmessage-list-chatmessagehostedcontents)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取托管内容](/graph/api/chatmessagehostedcontent-get)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天成员](/graph/api/conversationmember-list)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天成员](/graph/api/conversationmember-get)

>[!NOTE]
>[发送消息](/graph/api/channel-post-messages) API 不受保护。

要请求访问这些受保护的 API，请填写下述[请求表单](https://aka.ms/teamsgraph/requestaccess)。 我们在每周三审查访问请求，并在每周五部署批准，但美国的主要节假日周除外。在这些周中的提交将在下一个非节假日周进行处理。

如果除了表单，还想要提供其他信息，可与 [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) 联系。
