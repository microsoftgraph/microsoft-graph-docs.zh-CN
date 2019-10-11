---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1c7c8d18f59346387efbaa3c08de5794ad07ebab
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439882"
---
# <a name="protected-apis-in-microsoft-teams"></a>Microsoft Teams 中的受保护 API

Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。 除了权限和许可之外，这些 API 还需要进行额外的验证，然后才能使用。

以下是当前受保护的 API：
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出频道消息](/graph/api/channel-list-messages?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道增量中的聊天消息](/graph/api/chatmessage-delta.md)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道消息](/graph/api/channel-get-message?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出消息回复](/graph/api/channel-list-messagereplies?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取消息回复](/graph/api/channel-get-messagereply?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天中的消息](/graph/api/chatmessage-list?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天中的消息](/graph/api/chatmessage-get?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出所有托管内容](/graph/api/chatmessage-list-chatmessagehostedcontents.md)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取托管内容](/graph/api/chatmessagehostedcontent-get.md)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天成员](/graph/api/conversationmember-list.md)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天成员](/graph/api/conversationmember-get.md)

>[!NOTE]
>[发送消息](/graph/api/channel-post-messages?view=graph-rest-beta) API 不受保护。

要请求访问这些受保护的 API，请填写下述[请求表单](http://aka.ms/teamsgraph/requestaccess)。 我们每周三查看访问权限请求，每周五部署批准。
如果除了表单，还想要提供其他信息，可与 [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) 联系。
