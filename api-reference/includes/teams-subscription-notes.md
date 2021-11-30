---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 0c2faca238d1127462de5f70aadffd1ef3edd2d0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61132219"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

具有委派权限的 **chatMessage** 订阅不支持资源数据（**includeResourceData** 必须为 `false`），并且不需要 [加密](/graph/webhooks-with-resource-data)。 唯一的例外是 `/users/{id}/chats/getAllMessages` 资源（仅在 beta 版中可用），它支持资源数据，而不考虑权限类型。

具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。 如果未指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。 创建 **chatMessage** 订阅前，必须请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

> [!NOTE]
>`/teams/getAllMessages``/chats/getAllMessages`和[具有许可和付款要求](/graph/teams-licenses)。
> `/teams/getAllMessages` 支持 `/chats/getAllMessages` 和 `model=A` `model=B` 查询参数。
> 如果未指定模型，将使用[评估模式](/graph/teams-licenses#evaluation-mode-default-requirements)。

### <a name="conversationmember"></a>conversationMember

> [!NOTE]
>`/teams/getAllMembers``/chats/getAllMembers`和[具有许可和付款要求](/graph/teams-licenses)。
> `/teams/getAllMembers` 支持 `/chats/getAllMembers` 和 `model=A` `model=B` 查询参数。
> 如果未指定模型，将使用[评估模式](/graph/teams-licenses#evaluation-mode-default-requirements)。

### <a name="request-example"></a>请求示例

在 `model` 请求正文的 **resource** 属性中指定 query 参数。

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
