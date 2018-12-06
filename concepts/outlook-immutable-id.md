---
title: 获取 Outlook 资源不可变标识符
description: Outlook 项目 （邮件、 事件、 联系人、 任务） 具有有趣的行为，您可能已之一永远不会注意到或已导致重大失望： 更改其 Id。 它不会经常发生，仅当项目将被移动，但它可能会导致应用程序的更高版本用于存储脱机 Id 实际问题。 不可变标识符使您的应用程序获取不会更改项目的生存期内的 ID。
ms.openlocfilehash: a7b188c968ad6e0bf93f92ec99cb473075f29a4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091902"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="704a3-105">获取 Outlook 资源不可变标识符</span><span class="sxs-lookup"><span data-stu-id="704a3-105">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="704a3-106">Outlook 项目 （邮件、 事件、 联系人、 任务） 具有有趣的行为，您可能已之一永远不会注意到或已导致重大失望： 更改其 Id。</span><span class="sxs-lookup"><span data-stu-id="704a3-106">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="704a3-107">它不会经常发生，仅当项目将被移动，但它可能会导致应用程序的更高版本用于存储脱机 Id 实际问题。</span><span class="sxs-lookup"><span data-stu-id="704a3-107">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="704a3-108">不可变标识符使您的应用程序获取不会更改项目的生存期内的 ID。</span><span class="sxs-lookup"><span data-stu-id="704a3-108">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> <span data-ttu-id="704a3-109">**重要：** 不可变标识符是仅可供使用的 Microsoft Graph /beta 版本上。</span><span class="sxs-lookup"><span data-stu-id="704a3-109">**Important:** Immutable identifiers are only avaiable on the /beta version in Microsoft Graph.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="704a3-110">工作原理</span><span class="sxs-lookup"><span data-stu-id="704a3-110">How it works</span></span>

<span data-ttu-id="704a3-111">不可变 ID 是 Microsoft Graph 可选功能。</span><span class="sxs-lookup"><span data-stu-id="704a3-111">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="704a3-112">若要选择加入，您的应用程序需要发送 API 请求中的其他 HTTP 标头：</span><span class="sxs-lookup"><span data-stu-id="704a3-112">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="704a3-113">此标头仅适用于它是包含该请求。</span><span class="sxs-lookup"><span data-stu-id="704a3-113">This header only applies to the request it is included with.</span></span> <span data-ttu-id="704a3-114">如果您希望始终使用不可变 Id，您必须包含与每个 API 请求此标头。</span><span class="sxs-lookup"><span data-stu-id="704a3-114">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="704a3-115">不可变 Id 的生存期</span><span class="sxs-lookup"><span data-stu-id="704a3-115">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="704a3-116">只要项目将停留在同一邮箱，则不会更改项目的不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="704a3-116">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="704a3-117">也就是说，如果项目将被移动到另一个邮箱中的文件夹不会更改变 ID。</span><span class="sxs-lookup"><span data-stu-id="704a3-117">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="704a3-118">但是，如果将更改变 ID:</span><span class="sxs-lookup"><span data-stu-id="704a3-118">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="704a3-119">用户将项目移动到存档邮箱</span><span class="sxs-lookup"><span data-stu-id="704a3-119">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="704a3-120">用户导出 （到 PST，作为 MSG 文件等) 的项并重新将它导入到其邮箱</span><span class="sxs-lookup"><span data-stu-id="704a3-120">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="704a3-121">支持变 ID 的项目</span><span class="sxs-lookup"><span data-stu-id="704a3-121">Items that support immutable ID</span></span>

<span data-ttu-id="704a3-122">以下各项支持变 Id:</span><span class="sxs-lookup"><span data-stu-id="704a3-122">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="704a3-123">邮件资源类型</span><span class="sxs-lookup"><span data-stu-id="704a3-123">message resource type</span></span>](/graph/api/resources/message?view=graph-rest-beta)
- [<span data-ttu-id="704a3-124">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="704a3-124">attachment resource type</span></span>](/graph/api/resources/attachment?view=graph-rest-beta)
- [<span data-ttu-id="704a3-125">事件资源类型</span><span class="sxs-lookup"><span data-stu-id="704a3-125">event resource type</span></span>](/graph/api/resources/event?view=graph-rest-beta)
- [<span data-ttu-id="704a3-126">eventMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="704a3-126">eventMessage resource type</span></span>](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [<span data-ttu-id="704a3-127">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="704a3-127">contact resource type</span></span>](/graph/api/resources/contact?view=graph-rest-beta)
- [<span data-ttu-id="704a3-128">outlookTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="704a3-128">outlookTask resource type</span></span>](/graph/api/resources/outlooktask?view=graph-rest-beta)

<span data-ttu-id="704a3-129">（mailFolder、 日历等） 的容器类型不支持变 ID，但是它们的正则 Id 已常量。</span><span class="sxs-lookup"><span data-stu-id="704a3-129">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="704a3-130">更改通知不可变 ID</span><span class="sxs-lookup"><span data-stu-id="704a3-130">Immutable ID with change notifications</span></span>

<span data-ttu-id="704a3-131">您可以请求对 Microsoft Graph 发送变 Id 中的更改通知通过包括`Prefer: IdType="ImmutableId"`标头时[创建的订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="704a3-131">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span> <span data-ttu-id="704a3-132">创建没有标头的现有订阅将继续使用的默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="704a3-132">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="704a3-133">为了切换现有订阅使用不可变 Id，则必须删除并重新创建这些使用头。</span><span class="sxs-lookup"><span data-stu-id="704a3-133">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="704a3-134">不可变 ID 增量查询</span><span class="sxs-lookup"><span data-stu-id="704a3-134">Immutable ID with delta query</span></span>

<span data-ttu-id="704a3-135">您可以请求，Microsoft Graph 返回变 Id 中支持的资源类型的[增量查询响应](delta-query-overview.md)通过包括`Prefer: IdType="ImmutableId"`标头。</span><span class="sxs-lookup"><span data-stu-id="704a3-135">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="704a3-136">`nextLink`和`deltaLink`增量查询所返回的值都与两个 ID 格式，兼容，因此您的应用程序不需要重新同步利用变 id。</span><span class="sxs-lookup"><span data-stu-id="704a3-136">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="704a3-137">您可以使用标题获取变 Id 循序，并且可以[更新您的应用程序存储](#updating-existing-data)分开。</span><span class="sxs-lookup"><span data-stu-id="704a3-137">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="704a3-138">更新现有数据</span><span class="sxs-lookup"><span data-stu-id="704a3-138">Updating existing data</span></span>

<span data-ttu-id="704a3-139">如果您已经有了填充数千个正则 Id 的数据库，您可以为不可变格式使用[translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta)函数来迁移这些 Id。</span><span class="sxs-lookup"><span data-stu-id="704a3-139">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) function.</span></span> <span data-ttu-id="704a3-140">您可以提供最多 1000 Id 为目标格式转换的数组。</span><span class="sxs-lookup"><span data-stu-id="704a3-140">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> <span data-ttu-id="704a3-141">**注意：** 您还可以使用`translateExchangeIds`迁移到 Microsoft Graph 的 Exchange Web 服务应用程序。</span><span class="sxs-lookup"><span data-stu-id="704a3-141">**Note:** You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="704a3-142">示例</span><span class="sxs-lookup"><span data-stu-id="704a3-142">Example</span></span>

<span data-ttu-id="704a3-143">下面的示例将转换的普通图 ID 变图 id。</span><span class="sxs-lookup"><span data-stu-id="704a3-143">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="704a3-144">请求</span><span class="sxs-lookup"><span data-stu-id="704a3-144">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="704a3-145">响应</span><span class="sxs-lookup"><span data-stu-id="704a3-145">Response</span></span>

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