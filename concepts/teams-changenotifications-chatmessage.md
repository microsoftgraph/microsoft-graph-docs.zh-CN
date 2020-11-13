---
title: 使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知
description: 更改通知使你能够收听对频道或聊天中消息的更改
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1d9767a913b5fe5878cb1cc8e72ec9900fcec4ac
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000713"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="59677-103">使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知</span><span class="sxs-lookup"><span data-stu-id="59677-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="59677-104">更改通知使你能够订阅对[频道](/graph/api/resources/channel?preserve-view=true)或[聊天](/graph/api/resources/chat?preserve-view=true)中[消息](/graph/api/resources/chatMessage?preserve-view=true)的更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="59677-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="59677-105">更改通知允许你维护[订阅](/graph/api/resources/webhooks?preserve-view=true)，从而提供低延迟模式。</span><span class="sxs-lookup"><span data-stu-id="59677-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="59677-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="59677-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="59677-107">**注意：** 订阅的最长持续时间为 60 分钟；但是，订阅可以续订，直至呼叫方有权访问资源。</span><span class="sxs-lookup"><span data-stu-id="59677-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="59677-108">订阅租户级别的更改</span><span class="sxs-lookup"><span data-stu-id="59677-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="59677-109">若要跟踪与租户中的消息相关的所有更改，你可以使用租户级别的订阅来处理频道和聊天消息。</span><span class="sxs-lookup"><span data-stu-id="59677-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="59677-110">这需要你创建两个订阅：一个用于跟踪[频道](/graph/api/resources/channel?preserve-view=true)中的所有消息，另一个用于跟踪[聊天](/graph/api/resources/chat?preserve-view=true)中的所有消息。</span><span class="sxs-lookup"><span data-stu-id="59677-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="59677-111">跨频道订阅消息</span><span class="sxs-lookup"><span data-stu-id="59677-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="59677-112">若要跨租户中的频道获取所有消息和回复的更改通知，请订阅 `/teams/getAllMessages`。</span><span class="sxs-lookup"><span data-stu-id="59677-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="59677-113">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="59677-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="59677-114">权限</span><span class="sxs-lookup"><span data-stu-id="59677-114">Permissions</span></span>

|<span data-ttu-id="59677-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="59677-115">Permission type</span></span>      | <span data-ttu-id="59677-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59677-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59677-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-117">Delegated (work or school account)</span></span> | <span data-ttu-id="59677-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="59677-118">Not supported.</span></span> |
|<span data-ttu-id="59677-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59677-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="59677-120">Not supported.</span></span>    |
|<span data-ttu-id="59677-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="59677-121">Application</span></span> | <span data-ttu-id="59677-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="59677-122">ChannelMessage.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="59677-123">示例</span><span class="sxs-lookup"><span data-stu-id="59677-123">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="59677-124">跨聊天订阅消息</span><span class="sxs-lookup"><span data-stu-id="59677-124">Subscribe to messages across chats</span></span>

<span data-ttu-id="59677-125">若要跨租户中的聊天获取所有消息的更改通知，请订阅 `/chats/getAllMessages`。</span><span class="sxs-lookup"><span data-stu-id="59677-125">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="59677-126">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="59677-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="59677-127">权限</span><span class="sxs-lookup"><span data-stu-id="59677-127">Permissions</span></span>

|<span data-ttu-id="59677-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="59677-128">Permission type</span></span>      | <span data-ttu-id="59677-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59677-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59677-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-130">Delegated (work or school account)</span></span> | <span data-ttu-id="59677-131">不支持。</span><span class="sxs-lookup"><span data-stu-id="59677-131">Not supported.</span></span> |
|<span data-ttu-id="59677-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59677-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="59677-133">Not supported.</span></span>    |
|<span data-ttu-id="59677-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="59677-134">Application</span></span> | <span data-ttu-id="59677-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="59677-135">Chat.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="59677-136">示例</span><span class="sxs-lookup"><span data-stu-id="59677-136">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="59677-137">订阅频道中的消息</span><span class="sxs-lookup"><span data-stu-id="59677-137">Subscribe to messages in a channel</span></span>

<span data-ttu-id="59677-138">若要跟踪频道中的消息和回复，可在频道级别创建更改通知订阅。</span><span class="sxs-lookup"><span data-stu-id="59677-138">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="59677-139">为此，请订阅 `/teams{id}/channels/{id}/messages`。</span><span class="sxs-lookup"><span data-stu-id="59677-139">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="59677-140">此资源支持在 *仅限应用程序模式* 下[包括通知中的资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="59677-140">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="59677-141">频道级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。</span><span class="sxs-lookup"><span data-stu-id="59677-141">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="59677-142">权限</span><span class="sxs-lookup"><span data-stu-id="59677-142">Permissions</span></span>

|<span data-ttu-id="59677-143">权限类型</span><span class="sxs-lookup"><span data-stu-id="59677-143">Permission type</span></span>      | <span data-ttu-id="59677-144">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59677-144">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59677-145">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-145">Delegated (work or school account)</span></span> | <span data-ttu-id="59677-146">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="59677-146">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="59677-147">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59677-148">不支持。</span><span class="sxs-lookup"><span data-stu-id="59677-148">Not supported.</span></span>    |
|<span data-ttu-id="59677-149">应用程序</span><span class="sxs-lookup"><span data-stu-id="59677-149">Application</span></span> | <span data-ttu-id="59677-150">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="59677-150">ChannelMessage.Read.All</span></span> |

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="59677-151">示例 1：订阅频道中的所有消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="59677-151">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="59677-152">示例 2：订阅频道中包含特定文本的消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="59677-152">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="59677-153">以下请求将向订阅者发送包含 `Hello` 的消息。</span><span class="sxs-lookup"><span data-stu-id="59677-153">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="59677-154">示例 3：订阅频道中的消息（和回复），不含资源数据</span><span class="sxs-lookup"><span data-stu-id="59677-154">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="59677-155">订阅聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="59677-155">Subscribe to messages in a chat</span></span>

<span data-ttu-id="59677-156">若要跟踪聊天中的消息，你可以在聊天级别创建更改通知订阅。</span><span class="sxs-lookup"><span data-stu-id="59677-156">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="59677-157">为此，请订阅 `/chats{id}/messages`。</span><span class="sxs-lookup"><span data-stu-id="59677-157">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="59677-158">此资源支持在 *仅限应用程序模式* 下[包括通知中的资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="59677-158">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="59677-159">聊天级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。</span><span class="sxs-lookup"><span data-stu-id="59677-159">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="59677-160">权限</span><span class="sxs-lookup"><span data-stu-id="59677-160">Permissions</span></span>

|<span data-ttu-id="59677-161">权限类型</span><span class="sxs-lookup"><span data-stu-id="59677-161">Permission type</span></span>      | <span data-ttu-id="59677-162">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59677-162">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59677-163">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-163">Delegated (work or school account)</span></span> | <span data-ttu-id="59677-164">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="59677-164">Chat.Read</span></span> |
|<span data-ttu-id="59677-165">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59677-165">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59677-166">不支持。</span><span class="sxs-lookup"><span data-stu-id="59677-166">Not supported.</span></span>    |
|<span data-ttu-id="59677-167">应用程序</span><span class="sxs-lookup"><span data-stu-id="59677-167">Application</span></span> | <span data-ttu-id="59677-168">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="59677-168">Chat.Read.All</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="59677-169">示例 1：订阅聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="59677-169">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="59677-170">示例 2：订阅聊天中包含特定文本的消息</span><span class="sxs-lookup"><span data-stu-id="59677-170">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="59677-171">以下请求将向订阅者发送包含 `Hello` 的消息。</span><span class="sxs-lookup"><span data-stu-id="59677-171">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="59677-172">示例 3：订阅聊天中的消息（和回复），不含资源数据</span><span class="sxs-lookup"><span data-stu-id="59677-172">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

## <a name="see-also"></a><span data-ttu-id="59677-173">另请参阅</span><span class="sxs-lookup"><span data-stu-id="59677-173">See also</span></span>
- [<span data-ttu-id="59677-174">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="59677-174">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="59677-175">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="59677-175">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
