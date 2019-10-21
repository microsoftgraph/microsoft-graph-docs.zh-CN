---
title: 获取 Outlook 资源的不可变标识符
description: 借助不可变标识符，应用程序可为 Outlook 项获取在项生存期内保持不变的 ID。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: ca07e359f710d8538fe51f221895eca1beb08ec2
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "37439939"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="34209-103">获取 Outlook 资源的不可变标识符</span><span class="sxs-lookup"><span data-stu-id="34209-103">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="34209-104">Outlook 项（邮件、事件、联系人、任务）有一个有趣行为，你可能从未注意到或已给你带来了极大挫败感，即它们的 ID 会变。</span><span class="sxs-lookup"><span data-stu-id="34209-104">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="34209-105">虽然这一行为不是经常发生（只在项移动时才会发生），但对于脱机存储 ID 以供日后使用的应用来说，这可能会导致真正的问题出现。</span><span class="sxs-lookup"><span data-stu-id="34209-105">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="34209-106">借助不可变标识符，应用可以获取在项生存期内不变的 ID。</span><span class="sxs-lookup"><span data-stu-id="34209-106">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="34209-107">运作方式</span><span class="sxs-lookup"><span data-stu-id="34209-107">How it works</span></span>

<span data-ttu-id="34209-108">不可变 ID 是一项可选的 Microsoft Graph 功能。</span><span class="sxs-lookup"><span data-stu-id="34209-108">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="34209-109">若要选择使用此功能，应用必须在 API 请求中发送额外 HTTP 头：</span><span class="sxs-lookup"><span data-stu-id="34209-109">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="34209-110">此头仅适用于随附它的请求。</span><span class="sxs-lookup"><span data-stu-id="34209-110">This header only applies to the request it is included with.</span></span> <span data-ttu-id="34209-111">必须在每个 API 请求中随附此头，才能始终使用不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="34209-111">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="34209-112">不可变 ID 生存期</span><span class="sxs-lookup"><span data-stu-id="34209-112">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="34209-113">只要项一直在同一邮箱中，它的不可变 ID 就不变。</span><span class="sxs-lookup"><span data-stu-id="34209-113">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="34209-114">也就是说，即使项移到邮箱中的其他文件夹中，不可变 ID 也不变。</span><span class="sxs-lookup"><span data-stu-id="34209-114">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="34209-115">不过，不可变 ID 在以下情况下会变：</span><span class="sxs-lookup"><span data-stu-id="34209-115">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="34209-116">用户将该项移到存档邮箱中。</span><span class="sxs-lookup"><span data-stu-id="34209-116">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="34209-117">用户先将该项导出（到 PST 等，作为 MSG 文件），再将它重新导入邮箱。</span><span class="sxs-lookup"><span data-stu-id="34209-117">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>
- <span data-ttu-id="34209-118">用户发送草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="34209-118">The user sends a draft message.</span></span> <span data-ttu-id="34209-119">“已发送邮件”中副本的不可变 ID 与草稿邮件的不可变 ID 并不是同一 ID。</span><span class="sxs-lookup"><span data-stu-id="34209-119">The immutable ID of the copy in Sent Items will not be the same immutable ID of the draft message.</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="34209-120">支持不可变 ID 的项</span><span class="sxs-lookup"><span data-stu-id="34209-120">Items that support immutable ID</span></span>

<span data-ttu-id="34209-121">以下项支持不可变 ID：</span><span class="sxs-lookup"><span data-stu-id="34209-121">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="34209-122">message 资源类型</span><span class="sxs-lookup"><span data-stu-id="34209-122">message resource type</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="34209-123">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="34209-123">attachment resource type</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="34209-124">event 资源类型</span><span class="sxs-lookup"><span data-stu-id="34209-124">event resource type</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="34209-125">eventMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="34209-125">eventMessage resource type</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="34209-126">contact 资源类型</span><span class="sxs-lookup"><span data-stu-id="34209-126">contact resource type</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="34209-127">outlookTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="34209-127">outlookTask resource type</span></span>](/graph/api/resources/outlooktask)

<span data-ttu-id="34209-128">虽然容器类型（mailFolder、calendar 等）不支持不可变 ID，但其常规 ID 已是常量。</span><span class="sxs-lookup"><span data-stu-id="34209-128">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="34209-129">使用更改通知发送不可变 ID</span><span class="sxs-lookup"><span data-stu-id="34209-129">Immutable ID with change notifications</span></span>

<span data-ttu-id="34209-130">可以在[创建订阅](/graph/api/subscription-post-subscriptions)时添加 `Prefer: IdType="ImmutableId"` 头，从而请求 Microsoft Graph 在更改通知中发送不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="34209-130">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions).</span></span> <span data-ttu-id="34209-131">未使用此头创建的的现有订阅将继续使用默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="34209-131">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="34209-132">为了将现有订阅切换为使用不可变 ID，必须先删除它们，再使用此头重新创建它们。</span><span class="sxs-lookup"><span data-stu-id="34209-132">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="34209-133">使用 delta 查询发送不可变 ID</span><span class="sxs-lookup"><span data-stu-id="34209-133">Immutable ID with delta query</span></span>

<span data-ttu-id="34209-134">可以通过添加 `Prefer: IdType="ImmutableId"` 头，请求 Microsoft Graph 在受支持资源类型的 [delta 查询响应](delta-query-overview.md)中返回不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="34209-134">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="34209-135">由于 delta 查询返回的 `nextLink` 和 `deltaLink` 值与两种 ID 格式都兼容，因此应用无需重新同步，即可利用不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="34209-135">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="34209-136">可以使用此头在以后获取不可变 ID，也可以单独[更新应用的存储](#updating-existing-data)。</span><span class="sxs-lookup"><span data-stu-id="34209-136">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="34209-137">更新现有数据</span><span class="sxs-lookup"><span data-stu-id="34209-137">Updating existing data</span></span>

<span data-ttu-id="34209-138">如果已获取填充有数千个常规 ID 的数据库，可使用 [translateExchangeIds](/graph/api/user-translateexchangeids) 函数将这些 ID 迁移为不可变格式。</span><span class="sxs-lookup"><span data-stu-id="34209-138">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids) function.</span></span> <span data-ttu-id="34209-139">可以提供一组要转换为目标格式的 ID（最多 1000 个）。</span><span class="sxs-lookup"><span data-stu-id="34209-139">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> [!NOTE]
> <span data-ttu-id="34209-140">还可使用 `translateExchangeIds` 将 Exchange Web 服务应用程序迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="34209-140">Note: You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="34209-141">示例</span><span class="sxs-lookup"><span data-stu-id="34209-141">Example</span></span>

<span data-ttu-id="34209-142">下面的示例将普通 Graph ID 转换为不可变 Graph ID。</span><span class="sxs-lookup"><span data-stu-id="34209-142">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="34209-143">请求</span><span class="sxs-lookup"><span data-stu-id="34209-143">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="34209-144">响应</span><span class="sxs-lookup"><span data-stu-id="34209-144">Response</span></span>

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
