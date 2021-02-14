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

### <a name="chatmessage"></a><span data-ttu-id="0550f-101">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0550f-101">chatMessage</span></span>

<span data-ttu-id="0550f-102">具有委派权限的 **chatMessage** 订阅不支持资源数据（**includeResourceData** 必须为 `false`），并且不需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="0550f-102">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="0550f-103">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="0550f-103">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="0550f-104">如果未指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="0550f-104">Subscription creation will fail if [encryptionCertificate](/graph/api/resources/subscription) is not specified.</span></span> <span data-ttu-id="0550f-105">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="0550f-105">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="0550f-106">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="0550f-106">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="0550f-107">**注意：**</span><span class="sxs-lookup"><span data-stu-id="0550f-107">**Notes:**</span></span> 
>
><span data-ttu-id="0550f-108">`/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses) 的用户使用。</span><span class="sxs-lookup"><span data-stu-id="0550f-108">`/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="0550f-109">将来，Microsoft 可能需要你或你的客户根据通过 API 访问的数据量支付额外费用。</span><span class="sxs-lookup"><span data-stu-id="0550f-109">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>
>
><span data-ttu-id="0550f-110">`/chats/getAllMessages` 仅返回租户拥有的聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="0550f-110">`/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="0550f-111">如果聊天线程是由租户外部用户发起，则该聊天线程不属于租户，并且不会创建更改通知。</span><span class="sxs-lookup"><span data-stu-id="0550f-111">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>
