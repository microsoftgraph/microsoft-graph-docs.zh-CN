---
title: 获取 Outlook 资源的不可变标识符
description: Outlook 项（邮件、事件、联系人、任务）有一个有趣行为，你可能从未注意到或已给你带来了极大挫败感，即它们的 ID 会变。 虽然这一行为不是经常发生（只在项移动时才会发生），但对于脱机存储 ID 以供日后使用的应用来说，这可能会导致真正的问题出现。 借助不可变标识符，应用可以获取在项生存期内不变的 ID。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e88f4d457f76990dc3e6145ebf2730087ad2a74e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961713"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="5b52a-105">获取 Outlook 资源的不可变标识符</span><span class="sxs-lookup"><span data-stu-id="5b52a-105">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="5b52a-106">Outlook 项（邮件、事件、联系人、任务）有一个有趣行为，你可能从未注意到或已给你带来了极大挫败感，即它们的 ID 会变。</span><span class="sxs-lookup"><span data-stu-id="5b52a-106">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="5b52a-107">虽然这一行为不是经常发生（只在项移动时才会发生），但对于脱机存储 ID 以供日后使用的应用来说，这可能会导致真正的问题出现。</span><span class="sxs-lookup"><span data-stu-id="5b52a-107">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="5b52a-108">借助不可变标识符，应用可以获取在项生存期内不变的 ID。</span><span class="sxs-lookup"><span data-stu-id="5b52a-108">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> <span data-ttu-id="5b52a-109">**重要说明：** 不可变标识符仅适用于 Microsoft Graph /beta 版本。</span><span class="sxs-lookup"><span data-stu-id="5b52a-109">**Important:** Immutable identifiers are only avaiable on the /beta version in Microsoft Graph.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="5b52a-110">工作原理</span><span class="sxs-lookup"><span data-stu-id="5b52a-110">How it works</span></span>

<span data-ttu-id="5b52a-111">不可变 ID 是一项可选的 Microsoft Graph 功能。</span><span class="sxs-lookup"><span data-stu-id="5b52a-111">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="5b52a-112">若要选择使用此功能，应用必须在 API 请求中发送额外 HTTP 头：</span><span class="sxs-lookup"><span data-stu-id="5b52a-112">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="5b52a-113">此头仅适用于随附它的请求。</span><span class="sxs-lookup"><span data-stu-id="5b52a-113">This header only applies to the request it is included with.</span></span> <span data-ttu-id="5b52a-114">必须在每个 API 请求中随附此头，才能始终使用不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="5b52a-114">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="5b52a-115">不可变 ID 生存期</span><span class="sxs-lookup"><span data-stu-id="5b52a-115">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="5b52a-116">只要项一直在同一邮箱中，它的不可变 ID 就不变。</span><span class="sxs-lookup"><span data-stu-id="5b52a-116">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="5b52a-117">也就是说，即使项移到邮箱中的其他文件夹中，不可变 ID 也不变。</span><span class="sxs-lookup"><span data-stu-id="5b52a-117">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="5b52a-118">不过，不可变 ID 在以下情况下会变：</span><span class="sxs-lookup"><span data-stu-id="5b52a-118">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="5b52a-119">用户将项移到存档邮箱中</span><span class="sxs-lookup"><span data-stu-id="5b52a-119">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="5b52a-120">用户先将项导出（到 PST 等，作为 MSG 文件），再将它重新导入邮箱</span><span class="sxs-lookup"><span data-stu-id="5b52a-120">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="5b52a-121">支持不可变 ID 的项</span><span class="sxs-lookup"><span data-stu-id="5b52a-121">Items that support immutable ID</span></span>

<span data-ttu-id="5b52a-122">以下项支持不可变 ID：</span><span class="sxs-lookup"><span data-stu-id="5b52a-122">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="5b52a-123">message 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b52a-123">message resource type</span></span>](/graph/api/resources/message?view=graph-rest-beta)
- [<span data-ttu-id="5b52a-124">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b52a-124">attachment resource type</span></span>](/graph/api/resources/attachment?view=graph-rest-beta)
- [<span data-ttu-id="5b52a-125">event 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b52a-125">event resource type</span></span>](/graph/api/resources/event?view=graph-rest-beta)
- [<span data-ttu-id="5b52a-126">eventMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b52a-126">eventMessage resource type</span></span>](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [<span data-ttu-id="5b52a-127">contact 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b52a-127">contact resource type</span></span>](/graph/api/resources/contact?view=graph-rest-beta)
- [<span data-ttu-id="5b52a-128">outlookTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b52a-128">outlookTask resource type</span></span>](/graph/api/resources/outlooktask?view=graph-rest-beta)

<span data-ttu-id="5b52a-129">虽然容器类型（mailFolder、calendar 等）不支持不可变 ID，但其常规 ID 已是常量。</span><span class="sxs-lookup"><span data-stu-id="5b52a-129">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="5b52a-130">使用更改通知发送不可变 ID</span><span class="sxs-lookup"><span data-stu-id="5b52a-130">Immutable ID with change notifications</span></span>

<span data-ttu-id="5b52a-131">可以在[创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)时添加 `Prefer: IdType="ImmutableId"` 头，从而请求 Microsoft Graph 在更改通知中发送不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="5b52a-131">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span> <span data-ttu-id="5b52a-132">未使用此头创建的的现有订阅将继续使用默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="5b52a-132">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="5b52a-133">为了将现有订阅切换为使用不可变 ID，必须先删除它们，再使用此头重新创建它们。</span><span class="sxs-lookup"><span data-stu-id="5b52a-133">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="5b52a-134">使用 delta 查询发送不可变 ID</span><span class="sxs-lookup"><span data-stu-id="5b52a-134">Immutable ID with delta query</span></span>

<span data-ttu-id="5b52a-135">可以通过添加 `Prefer: IdType="ImmutableId"` 头，请求 Microsoft Graph 在受支持资源类型的 [delta 查询响应](delta-query-overview.md)中返回不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="5b52a-135">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="5b52a-136">由于 delta 查询返回的 `nextLink` 和 `deltaLink` 值与两种 ID 格式都兼容，因此应用无需重新同步，即可利用不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="5b52a-136">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="5b52a-137">可以使用此头在以后获取不可变 ID，也可以单独[更新应用的存储](#updating-existing-data)。</span><span class="sxs-lookup"><span data-stu-id="5b52a-137">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="5b52a-138">更新现有数据</span><span class="sxs-lookup"><span data-stu-id="5b52a-138">Updating existing data</span></span>

<span data-ttu-id="5b52a-139">如果已获取填充有数千个常规 ID 的数据库，可使用 [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) 函数将这些 ID 迁移为不可变格式。</span><span class="sxs-lookup"><span data-stu-id="5b52a-139">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) function.</span></span> <span data-ttu-id="5b52a-140">可以提供一组要转换为目标格式的 ID（最多 1000 个）。</span><span class="sxs-lookup"><span data-stu-id="5b52a-140">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> <span data-ttu-id="5b52a-141">**注意：** 也可以使用 `translateExchangeIds` 将 Exchange Web 服务应用迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="5b52a-141">**Note:** You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="5b52a-142">示例</span><span class="sxs-lookup"><span data-stu-id="5b52a-142">Example</span></span>

<span data-ttu-id="5b52a-143">下面的示例将普通 Graph ID 转换为不可变 Graph ID。</span><span class="sxs-lookup"><span data-stu-id="5b52a-143">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="5b52a-144">请求</span><span class="sxs-lookup"><span data-stu-id="5b52a-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="5b52a-145">响应</span><span class="sxs-lookup"><span data-stu-id="5b52a-145">Response</span></span>

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```
