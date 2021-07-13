---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.openlocfilehash: f3854b06c7d4dc584a922f9c454947785b74947f
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2021
ms.locfileid: "53005775"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

具有委派权限的 **chatMessage** 订阅不支持资源数据（**includeResourceData** 必须为 `false`），并且不需要 [加密](/graph/webhooks-with-resource-data)。

具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。 如果未指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。 创建 **chatMessage** 订阅前，必须请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。 

> **注意：** 
>
>`/teams/getAllMessages` 和 `/chats/getAllMessages` 可供具有所需 [许可证](https://aka.ms/teams-changenotification-licenses) 的用户使用。将来，Microsoft 可能会要求你或你的客户根据通过 API 访问的数据量支付额外费用。
