---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.openlocfilehash: f2def5f5a22267146d5b3005cd2f9be82e1d0db9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50243135"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

具有委派权限的 **chatMessage** 订阅不支持资源数据（**includeResourceData** 必须为 `false`），并且不需要 [加密](/graph/webhooks-with-resource-data)。

具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。 如果未指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。 创建 **chatMessage** 订阅前，必须请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。 

> **注意：** 
>
>`/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses) 的用户使用。
将来，Microsoft 可能需要你或你的客户根据通过 API 访问的数据量支付额外费用。
>
>`/chats/getAllMessages` 仅返回租户拥有的聊天中的消息。 如果聊天线程是由租户外部用户发起，则该聊天线程不属于租户，并且不会创建更改通知。
