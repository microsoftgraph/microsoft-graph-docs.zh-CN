---
title: 使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知
description: 更改通知使你能够收听对频道或聊天中消息的更改
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 186599391599c7ac77f637bcc910339f3087c999
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101879"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="ec47e-103">使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知</span><span class="sxs-lookup"><span data-stu-id="ec47e-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="ec47e-104">更改通知使你能够订阅对[频道](/graph/api/resources/channel?preserve-view=true)或[聊天](/graph/api/resources/chat?preserve-view=true)中[消息](/graph/api/resources/chatMessage?preserve-view=true)的更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="ec47e-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="ec47e-105">更改通知允许你维护[订阅](/graph/api/resources/webhooks?preserve-view=true)，从而提供低延迟模式。</span><span class="sxs-lookup"><span data-stu-id="ec47e-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="ec47e-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="ec47e-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="ec47e-107">**注意：** 订阅的最长持续时间为 60 分钟；但是，订阅可以续订，直至呼叫方有权访问资源。</span><span class="sxs-lookup"><span data-stu-id="ec47e-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="ec47e-108">订阅租户级别的更改</span><span class="sxs-lookup"><span data-stu-id="ec47e-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="ec47e-109">若要跟踪与租户中的消息相关的所有更改，你可以使用租户级别的订阅来处理频道和聊天消息。</span><span class="sxs-lookup"><span data-stu-id="ec47e-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="ec47e-110">这需要你创建两个订阅：一个用于跟踪[频道](/graph/api/resources/channel?preserve-view=true)中的所有消息，另一个用于跟踪[聊天](/graph/api/resources/chat?preserve-view=true)中的所有消息。</span><span class="sxs-lookup"><span data-stu-id="ec47e-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="ec47e-111">跨频道订阅消息</span><span class="sxs-lookup"><span data-stu-id="ec47e-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="ec47e-112">若要跨租户中的频道获取所有消息和回复的更改通知，请订阅 `/teams/getAllMessages`。</span><span class="sxs-lookup"><span data-stu-id="ec47e-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="ec47e-113">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="ec47e-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="ec47e-114">权限</span><span class="sxs-lookup"><span data-stu-id="ec47e-114">Permissions</span></span>

|<span data-ttu-id="ec47e-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec47e-115">Permission type</span></span>      | <span data-ttu-id="ec47e-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec47e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec47e-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ec47e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec47e-118">Not supported.</span></span> |
|<span data-ttu-id="ec47e-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec47e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec47e-120">Not supported.</span></span>    |
|<span data-ttu-id="ec47e-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec47e-121">Application</span></span> | <span data-ttu-id="ec47e-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec47e-122">ChannelMessage.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="ec47e-123">示例</span><span class="sxs-lookup"><span data-stu-id="ec47e-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="ec47e-124">跨聊天订阅消息</span><span class="sxs-lookup"><span data-stu-id="ec47e-124">Subscribe to messages across chats</span></span>

<span data-ttu-id="ec47e-125">若要跨租户中的聊天获取所有消息的更改通知，请订阅 `/chats/getAllMessages`。</span><span class="sxs-lookup"><span data-stu-id="ec47e-125">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="ec47e-126">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="ec47e-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="ec47e-127">权限</span><span class="sxs-lookup"><span data-stu-id="ec47e-127">Permissions</span></span>

|<span data-ttu-id="ec47e-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec47e-128">Permission type</span></span>      | <span data-ttu-id="ec47e-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec47e-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec47e-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-130">Delegated (work or school account)</span></span> | <span data-ttu-id="ec47e-131">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec47e-131">Not supported.</span></span> |
|<span data-ttu-id="ec47e-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec47e-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec47e-133">Not supported.</span></span>    |
|<span data-ttu-id="ec47e-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec47e-134">Application</span></span> | <span data-ttu-id="ec47e-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec47e-135">Chat.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="ec47e-136">示例</span><span class="sxs-lookup"><span data-stu-id="ec47e-136">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="ec47e-137">订阅频道中的消息</span><span class="sxs-lookup"><span data-stu-id="ec47e-137">Subscribe to messages in a channel</span></span>

<span data-ttu-id="ec47e-138">若要跟踪频道中的消息和回复，可在频道级别创建更改通知订阅。</span><span class="sxs-lookup"><span data-stu-id="ec47e-138">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="ec47e-139">为此，请订阅 `/teams{id}/channels/{id}/messages`。</span><span class="sxs-lookup"><span data-stu-id="ec47e-139">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="ec47e-140">此资源支持在 *仅限应用程序模式* 下 [包括通知中的资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="ec47e-140">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="ec47e-141">频道级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。</span><span class="sxs-lookup"><span data-stu-id="ec47e-141">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="ec47e-142">权限</span><span class="sxs-lookup"><span data-stu-id="ec47e-142">Permissions</span></span>

|<span data-ttu-id="ec47e-143">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec47e-143">Permission type</span></span>      | <span data-ttu-id="ec47e-144">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec47e-144">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec47e-145">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-145">Delegated (work or school account)</span></span> | <span data-ttu-id="ec47e-146">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec47e-146">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="ec47e-147">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec47e-148">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec47e-148">Not supported.</span></span>    |
|<span data-ttu-id="ec47e-149">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec47e-149">Application</span></span> | <span data-ttu-id="ec47e-150">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="ec47e-150">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> |

><span data-ttu-id="ec47e-151">**注意：** ChannelMessage.Read.Group 作为 [资源特定许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)的一部分受支持。</span><span class="sxs-lookup"><span data-stu-id="ec47e-151">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="ec47e-152">示例 1：订阅频道中的所有消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="ec47e-152">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="ec47e-153">示例 2：订阅频道中包含特定文本的消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="ec47e-153">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="ec47e-154">以下请求将向订阅者发送包含 `Hello` 的消息。</span><span class="sxs-lookup"><span data-stu-id="ec47e-154">The following request will send messages that contain `Hello` to the subscriber.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="ec47e-155">示例 3：订阅频道中的消息（和回复），不含资源数据</span><span class="sxs-lookup"><span data-stu-id="ec47e-155">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="ec47e-156">示例 4：订阅频道中提到特定用户的消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="ec47e-156">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="ec47e-157">要仅获得提到特定用户的消息，你可以在查询中指定用户的 ID（在此示例中为 `9a6eb4d1-826b-48b1-9627-b50836c8fee9`）。</span><span class="sxs-lookup"><span data-stu-id="ec47e-157">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="ec47e-158">订阅聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="ec47e-158">Subscribe to messages in a chat</span></span>

<span data-ttu-id="ec47e-159">若要跟踪聊天中的消息，你可以在聊天级别创建更改通知订阅。</span><span class="sxs-lookup"><span data-stu-id="ec47e-159">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="ec47e-160">为此，请订阅 `/chats{id}/messages`。</span><span class="sxs-lookup"><span data-stu-id="ec47e-160">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="ec47e-161">此资源支持在 *仅限应用程序模式* 下 [包括通知中的资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="ec47e-161">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="ec47e-162">聊天级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。</span><span class="sxs-lookup"><span data-stu-id="ec47e-162">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="ec47e-163">**注意。**</span><span class="sxs-lookup"><span data-stu-id="ec47e-163">**Note.**</span></span> <span data-ttu-id="ec47e-164">订阅聊天中的消息目前在预览中。</span><span class="sxs-lookup"><span data-stu-id="ec47e-164">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="ec47e-165">权限</span><span class="sxs-lookup"><span data-stu-id="ec47e-165">Permissions</span></span>

|<span data-ttu-id="ec47e-166">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec47e-166">Permission type</span></span>      | <span data-ttu-id="ec47e-167">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec47e-167">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec47e-168">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-168">Delegated (work or school account)</span></span> | <span data-ttu-id="ec47e-169">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="ec47e-169">Chat.Read</span></span> |
|<span data-ttu-id="ec47e-170">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec47e-170">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec47e-171">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec47e-171">Not supported.</span></span>    |
|<span data-ttu-id="ec47e-172">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec47e-172">Application</span></span> | <span data-ttu-id="ec47e-173">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec47e-173">Chat.Read.All</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="ec47e-174">示例 1：订阅聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="ec47e-174">Example 1: Subscribe to messages in a chat</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="ec47e-175">示例 2：订阅聊天中包含特定文本的消息</span><span class="sxs-lookup"><span data-stu-id="ec47e-175">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="ec47e-176">以下请求将向订阅者发送包含 `Hello` 的消息。</span><span class="sxs-lookup"><span data-stu-id="ec47e-176">The following request will send messages that contain `Hello` to the subscriber.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="ec47e-177">示例 3：订阅聊天中的消息（和回复），不含资源数据</span><span class="sxs-lookup"><span data-stu-id="ec47e-177">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="ec47e-178">示例 4：订阅聊天中提到特定用户的消息</span><span class="sxs-lookup"><span data-stu-id="ec47e-178">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="ec47e-179">要仅获得提到特定用户的消息，你可以在查询中指定用户的 ID（在此示例中为 `9a6eb4d1-826b-48b1-9627-b50836c8fee9`）。</span><span class="sxs-lookup"><span data-stu-id="ec47e-179">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="notification-payloads"></a><span data-ttu-id="ec47e-180">通知负载</span><span class="sxs-lookup"><span data-stu-id="ec47e-180">Notification payloads</span></span>

<span data-ttu-id="ec47e-181">根据你的订阅，你可以获取包含或不含资源数据的通知。</span><span class="sxs-lookup"><span data-stu-id="ec47e-181">Depending on your subscription, you can either get the notification with resource data, or without it.</span></span> <span data-ttu-id="ec47e-182">通过订阅资源数据，你将在收到通知的同时获得消息负载，而无需回调并获取内容。</span><span class="sxs-lookup"><span data-stu-id="ec47e-182">Subscribing with resource data allows you to get the message payload along with the notification, removing the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="ec47e-183">包含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="ec47e-183">Notifications with resource data</span></span>

<span data-ttu-id="ec47e-184">对于包含资源数据的通知，负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="ec47e-184">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="ec47e-185">此负载适用于在聊天中发送的消息。</span><span class="sxs-lookup"><span data-stu-id="ec47e-185">This payload is for a message sent in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="ec47e-186">有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="ec47e-186">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="ec47e-187">解密的通知负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="ec47e-187">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="ec47e-188">该负载符合 [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="ec47e-188">The payload conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="ec47e-189">该负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="ec47e-189">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="ec47e-190">不含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="ec47e-190">Notifications without resource data</span></span>

<span data-ttu-id="ec47e-191">不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取消息内容。</span><span class="sxs-lookup"><span data-stu-id="ec47e-191">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="ec47e-192">订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。</span><span class="sxs-lookup"><span data-stu-id="ec47e-192">Subscriptions for notifications without resource data do not require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="ec47e-193">该负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="ec47e-193">The payload looks like the following.</span></span> <span data-ttu-id="ec47e-194">此负载适用于在频道中发送的消息。</span><span class="sxs-lookup"><span data-stu-id="ec47e-194">This payload is for a message sent in a channel.</span></span>

```json
 {
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```

<span data-ttu-id="ec47e-195">**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息负载。</span><span class="sxs-lookup"><span data-stu-id="ec47e-195">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="ec47e-196">GET 调用将始终返回消息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="ec47e-196">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="ec47e-197">如果在发送通知和检索消息之间更改了消息，则该操作将返回更新的消息。</span><span class="sxs-lookup"><span data-stu-id="ec47e-197">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="ec47e-198">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ec47e-198">See also</span></span>
- [<span data-ttu-id="ec47e-199">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="ec47e-199">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="ec47e-200">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="ec47e-200">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
