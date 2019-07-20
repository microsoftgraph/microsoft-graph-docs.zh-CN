---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ebf0bbda324f62c6413bbe3d70ade33a5052da0d
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778759"
---
# <a name="protected-apis-in-microsoft-teams"></a>Microsoft Teams 中的受保护 API

Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。 除了权限和许可之外，这些 API 还需要进行额外的验证，然后才能使用。

以下是当前受保护的 API：
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出频道消息](/graph/api/channel-list-messages?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道消息](/graph/api/channel-get-message?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出消息回复](/graph/api/channel-list-messagereplies?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取消息回复](/graph/api/channel-get-messagereply?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天中的消息](/graph/api/chatmessage-list?view=graph-rest-beta)
* 使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天中的消息](/graph/api/chatmessage-get?view=graph-rest-beta)

若要请求对这些受保护 API 的访问权限，请完成以下[请求表单](http://aka.ms/teamsgraph/requestaccess)。 我们每周都会查看一次访问权限请求。 如果想要在表单之外提供其他信息，可与 [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) 联系。
