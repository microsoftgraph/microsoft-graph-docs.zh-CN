---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 9a1c86904767b9cb9f36082d06733b36449fe920
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59763407"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

具有委派权限的 **chatMessage** 订阅不支持资源数据（**includeResourceData** 必须为 `false`），并且不需要 [加密](/graph/webhooks-with-resource-data)。 唯一的例外是 `/users/{id}/chats/getAllMessages` 资源（仅在 beta 版中可用），它支持资源数据，而不考虑权限类型。

具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。 如果未指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。 创建 **chatMessage** 订阅前，必须请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

> [!NOTE]
> `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供具有所需 [许可证](https://aka.ms/teams-changenotification-licenses) 的用户使用。将来，Microsoft 可能会要求你或你的客户根据通过 API 访问的数据量支付额外费用。
