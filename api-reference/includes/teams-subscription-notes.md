---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 6e5f62d52969dcc1b332b2cd6e5f02f318c8b6a9
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65135151"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

可以指定 **chatMessage** 订阅以包含资源数据。 如果指定为包含资源数据（将 **includeResourceData** 设置为 `true`），则需要 [encryption](/graph/webhooks-with-resource-data)。 如果没有为此类订阅指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。 在可以使用应用程序权限创建 **chatMessage** 订阅之前，可能需要请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

必须使用 `Prefer: include-unknown-enum-members` 请求标头以 **chatMessage** **messageType** [evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) 中获取以下值：适用于 `/teams/{id}/channels/{id}/messages` 和 `/chats/{id}/messages` 的 `systemEventMessage`。

> [!NOTE]
>`/teams/getAllMessages`、`/chats/getAllMessages`、`/me/chats/getAllMessages`和`/users/{id}/chats/getAllMessages`具有[许可和付款要求](/graph/teams-licenses)。
> `/teams/getAllMessages`和`/chats/getAllMessages`支持`model=A`和`model=B`查询参数，`/me/chats/getAllMessages`和`/users/{id}/chats/getAllMessages`仅支持`model=B`。
> 如果未指定模型，将使用[评估模式](/graph/teams-licenses#evaluation-mode-default-requirements)。

### <a name="conversationmember"></a>conversationMember

> [!NOTE]
>`/teams/getAllMembers` 和 `/chats/getAllMembers` 具有 [许可和付款要求](/graph/teams-licenses)。
> `/teams/getAllMembers` 和 `/chats/getAllMembers` 同时支持 `model=A` 和 `model=B` 查询参数。
> 如果未指定模型，将使用[评估模式](/graph/teams-licenses#evaluation-mode-default-requirements)。

#### <a name="request-example"></a>请求示例

在请求正文中的 **资源** 内指定 `model` 查询参数。

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "chats/getAllMessages?model=A",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
