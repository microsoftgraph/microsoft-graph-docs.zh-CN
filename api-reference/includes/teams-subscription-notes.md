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

### <a name="chatmessage"></a><span data-ttu-id="0abbb-101">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0abbb-101">chatMessage</span></span>

<span data-ttu-id="0abbb-102">具有委派权限的 **chatMessage** 订阅不支持资源数据（**includeResourceData** 必须为 `false`），并且不需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="0abbb-102">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="0abbb-103">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="0abbb-103">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="0abbb-104">如果未指定 [encryptionCertificate](/graph/api/resources/subscription)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="0abbb-104">Subscription creation will fail if [encryptionCertificate](/graph/api/resources/subscription) is not specified.</span></span> <span data-ttu-id="0abbb-105">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="0abbb-105">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="0abbb-106">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="0abbb-106">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="0abbb-107">**注意：**</span><span class="sxs-lookup"><span data-stu-id="0abbb-107">**Notes:**</span></span> 
>
><span data-ttu-id="0abbb-p102">`/teams/getAllMessages` 和 `/chats/getAllMessages` 可供具有所需 [许可证](https://aka.ms/teams-changenotification-licenses) 的用户使用。将来，Microsoft 可能会要求你或你的客户根据通过 API 访问的数据量支付额外费用。</span><span class="sxs-lookup"><span data-stu-id="0abbb-p102">`/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses). In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>
