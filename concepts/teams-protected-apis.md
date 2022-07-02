---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中访问敏感数据的 Microsoft Teams API 被视为受保护的 API，需要进行其他验证才能使用它们。
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: a8c7de28d1ecd5784e69e2cc4774802282b8bd24
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577810"
---
# <a name="protected-apis-in-microsoft-teams"></a>Microsoft Teams 中的受保护 API

Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。 除了权限和同意之外，这些 API 还需要进行其他验证，然后才能使用。

以下 API 当前受保护，并且所有 API 都使用 [Microsoft Graph 应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)：

* [列出频道消息](/graph/api/channel-list-messages)
* [获取频道 delta 中的 chatMessages](/graph/api/chatmessage-delta)
* [获取频道消息](/graph/api/chatmessage-get)
* [创建新频道消息的订阅](/graph/api/subscription-post-subscriptions)
* [列出消息回复](/graph/api/chatmessage-list-replies)
* [获取消息回复](/graph/api/chatmessage-get)
* （列表聊天不存在，无论是否具有受保护的 API 访问权限）
* [列出聊天中的消息](/graph/api/chat-list-messages)
* [获取聊天中的消息](/graph/api/chatmessage-get)
* [创建新聊天消息的订阅](/graph/api/subscription-post-subscriptions)
* [列出所有托管内容](/graph/api/chatmessage-list-hostedcontents)
* [获取托管内容](/graph/api/chatmessagehostedcontent-get)
* [获取已删除团队中的消息](/graph/api/deletedteam-getallmessages)

> [!NOTE]
> [发送消息](/graph/api/channel-post-messages) API 不受保护。

## <a name="request-access-to-protected-apis"></a>请求访问受保护的 API

要请求访问这些受保护的 API，请填写下述[请求表单](https://forms.office.com/r/v3qjyzBCxD)。 我们通常每周三查看访问请求，并在每周五或周一部署审批，但美国主要节假日除外。在这些周内提交的请求将在接下来的非节假日周处理。

若要验证请求是否已获得批准，请于下一个适用的星期一测试应用程序访问权限。 如果我们对请求有其他问题，我们将与表单中指定的电子邮件联系。

## <a name="see-also"></a>另请参阅

* [Microsoft Teams API 概述](teams-concept-overview.md)