---
title: 使用 Microsoft Graph 中的通话记录 API
description: Microsoft Graph 通话记录 API 可用于检索组织内的通话和联机会议的使用情况和诊断数据。
author: stephenjust
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 9b48b3d7f0265c44bc62c3ee2182353343692a10
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507801"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a><span data-ttu-id="07d1a-103">使用 Microsoft Graph 中的通话记录 API</span><span class="sxs-lookup"><span data-stu-id="07d1a-103">Working with the call records API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07d1a-104">通话记录提供了使用 Microsoft Teams 或 Skype for Business 时组织内发生的通话和联机会议的使用情况和诊断信息。</span><span class="sxs-lookup"><span data-stu-id="07d1a-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="07d1a-105">可使用通话记录 API 来订阅通话记录，并按 ID 查找通话记录。</span><span class="sxs-lookup"><span data-stu-id="07d1a-105">You can use the call records APIs to subscribe to call records and look up call records by IDs.</span></span>

<span data-ttu-id="07d1a-106">通话记录 API 在 OData 子命名空间中定，`microsoft.graph.callRecords`。</span><span class="sxs-lookup"><span data-stu-id="07d1a-106">The call records API is defined in the OData sub-namespace, `microsoft.graph.callRecords`.</span></span>

## <a name="key-resource-types"></a><span data-ttu-id="07d1a-107">重要资源类型</span><span class="sxs-lookup"><span data-stu-id="07d1a-107">Key resource types</span></span>

| <span data-ttu-id="07d1a-108">Resource</span><span class="sxs-lookup"><span data-stu-id="07d1a-108">Resource</span></span> | <span data-ttu-id="07d1a-109">Methods</span><span class="sxs-lookup"><span data-stu-id="07d1a-109">Methods</span></span> |
| :-- | :-- |
| [<span data-ttu-id="07d1a-110">callRecord</span><span class="sxs-lookup"><span data-stu-id="07d1a-110">callRecord</span></span>](callrecords-callrecord.md) | [<span data-ttu-id="07d1a-111">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="07d1a-111">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |
| [<span data-ttu-id="07d1a-112">Session</span><span class="sxs-lookup"><span data-stu-id="07d1a-112">session</span></span>](callrecords-session.md) | [<span data-ttu-id="07d1a-113">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="07d1a-113">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |
| [<span data-ttu-id="07d1a-114">segment</span><span class="sxs-lookup"><span data-stu-id="07d1a-114">segment</span></span>](callrecords-segment.md) | [<span data-ttu-id="07d1a-115">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="07d1a-115">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |

## <a name="call-record-structure"></a><span data-ttu-id="07d1a-116">呼叫记录结构</span><span class="sxs-lookup"><span data-stu-id="07d1a-116">Call record structure</span></span>

<span data-ttu-id="07d1a-117">[callRecord](callrecords-callrecord.md) 实体表示多个参与者之间的单个对等呼叫或群组呼叫，有时称为联机会议。</span><span class="sxs-lookup"><span data-stu-id="07d1a-117">The [callRecord](callrecords-callrecord.md) entity represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

<span data-ttu-id="07d1a-118">对等呼叫包含呼叫中两个参与者之间的单个 [session](callrecords-session.md)。</span><span class="sxs-lookup"><span data-stu-id="07d1a-118">A peer-to-peer call contains a single [session](callrecords-session.md) between the two participants in the call.</span></span> <span data-ttu-id="07d1a-119">群组呼叫包含一个或多个 **session** 实体。</span><span class="sxs-lookup"><span data-stu-id="07d1a-119">Group calls contain one or more **session** entities.</span></span> <span data-ttu-id="07d1a-120">在群组呼叫中，每个 **session** 都介于参与者和服务终结点之间。</span><span class="sxs-lookup"><span data-stu-id="07d1a-120">In a group call, each **session** is between the participant and a service endpoint.</span></span>

<span data-ttu-id="07d1a-121">每个 **session** 都包含一个或多个 [segment](callrecords-segment.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="07d1a-121">Each **session** contains one or more [segment](callrecords-segment.md) entities.</span></span> <span data-ttu-id="07d1a-122">**segment** 表示两个[终结点](callrecords-endpoint.md)之间的媒体链接。</span><span class="sxs-lookup"><span data-stu-id="07d1a-122">A **segment** represents a media link between two [endpoints](callrecords-endpoint.md).</span></span> <span data-ttu-id="07d1a-123">对于大多数呼叫，每个 **session** 仅显示一个 **segment**，但有时可能会有一个或多个中间**终结点**。</span><span class="sxs-lookup"><span data-stu-id="07d1a-123">For most calls, only one **segment** will be present for each **session**, however sometimes there may be one or more intermediate **endpoints**.</span></span>

![表示完整通话记录的数据结构的图像](/graph/images/callrecords-structure.png)

<span data-ttu-id="07d1a-125">在上图中，数字表示每种类型可以有多少个子类型。</span><span class="sxs-lookup"><span data-stu-id="07d1a-125">In the diagram above, the numbers denote how many children of each type can be present.</span></span> <span data-ttu-id="07d1a-126">例如，**callRecord** 与 **session** 之间的 1..N 关系意味着一个 **callRecord** 实例可以包含一个或多个 **session** 实例。</span><span class="sxs-lookup"><span data-stu-id="07d1a-126">For example, a 1..N relationship between a **callRecord** and a **session** means one **callRecord** instance can contain one or more **session** instances.</span></span> <span data-ttu-id="07d1a-127">同样，**segment** 与 **media** 之间的 1..N 关系意味着一个 **segment** 实例可以包含一个或多个 [media](callrecords-media.md) 流。</span><span class="sxs-lookup"><span data-stu-id="07d1a-127">Similarly, a 1..N relationship between a **segment** and a **media** means one **segment** instance can contain one or more [media](callrecords-media.md) streams.</span></span>

## <a name="see-also"></a><span data-ttu-id="07d1a-128">另请参阅</span><span class="sxs-lookup"><span data-stu-id="07d1a-128">See also</span></span>

- [<span data-ttu-id="07d1a-129">Webhook 订阅</span><span class="sxs-lookup"><span data-stu-id="07d1a-129">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-beta)
