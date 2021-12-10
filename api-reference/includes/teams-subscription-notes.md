---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: e9b65c0ed6c82e94a38bbeb08b208fbe24d60176
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390807"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

具有委派权限的 **chatMessage** 订阅不支持资源数据（**includeResourceData** 必须为 `false`），并且不需要 [加密](/graph/webhooks-with-resource-data)。 唯一的例外是 `/users/{id}/chats/getAllMessages` 资源（仅在 beta 版中可用），它支持资源数据，而不考虑权限类型。

具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。 如果未指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。 创建 **chatMessage** 订阅前，必须请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

必须使用 `Prefer: include-unknown-enum-members` 请求标头以 **chatMessage** **messageType** [evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) 中获取以下值：适用于 `/teams/{id}/channels/{id}/messages` 和 `/chats/{id}/messages` 的 `systemEventMessage`。

> [!NOTE]
>`/teams/getAllMessages` 和 `/chats/getAllMessages` 具有 [许可和付款要求](/graph/teams-licenses)。
> `/teams/getAllMessages` 和 `/chats/getAllMessages` 同时支持 `model=A` 和 `model=B` 查询参数。
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
