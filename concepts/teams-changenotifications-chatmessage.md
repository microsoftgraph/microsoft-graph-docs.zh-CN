---
title: 使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知
description: 更改通知使你能够收听对频道或聊天中消息的更改
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 78718b1b486231ae2549323433312aa878806210
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941422"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="aec14-103">使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知</span><span class="sxs-lookup"><span data-stu-id="aec14-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="aec14-104">更改通知使你能够订阅频道或聊天中消息的更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="aec14-104">Change notifications enable you to subscribe to changes (create, update, and delete) to messages in a channel or chat.</span></span> <span data-ttu-id="aec14-105">更改通知允许你维护订阅，从而提供低延迟模式。</span><span class="sxs-lookup"><span data-stu-id="aec14-105">Change notifications provide a low latency model by allowing you to maintain a subscription.</span></span> <span data-ttu-id="aec14-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="aec14-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="aec14-107">订阅租户级别的更改</span><span class="sxs-lookup"><span data-stu-id="aec14-107">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="aec14-108">若要跟踪与租户中的消息相关的所有更改，你可以使用租户级别的订阅来处理频道和聊天消息。</span><span class="sxs-lookup"><span data-stu-id="aec14-108">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="aec14-109">这需要你创建两个订阅：一个用于跟踪[频道](/graph/api/resources/channel?preserve-view=true)中的所有消息，另一个用于跟踪[聊天](/graph/api/resources/chat?preserve-view=true)中的所有消息。</span><span class="sxs-lookup"><span data-stu-id="aec14-109">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="aec14-110">跨频道订阅消息</span><span class="sxs-lookup"><span data-stu-id="aec14-110">Subscribe to messages across channels</span></span>

<span data-ttu-id="aec14-111">若要跨租户中的频道获取所有消息和回复的更改通知，请订阅 `/teams/getAllMessages`。</span><span class="sxs-lookup"><span data-stu-id="aec14-111">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="aec14-112">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="aec14-112">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="aec14-113">权限</span><span class="sxs-lookup"><span data-stu-id="aec14-113">Permissions</span></span>

|<span data-ttu-id="aec14-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="aec14-114">Permission type</span></span>      | <span data-ttu-id="aec14-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aec14-115">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="aec14-116">支持的版本</span><span class="sxs-lookup"><span data-stu-id="aec14-116">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="aec14-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-117">Delegated (work or school account)</span></span> | <span data-ttu-id="aec14-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-118">Not supported.</span></span> | <span data-ttu-id="aec14-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-119">Not supported.</span></span> |
|<span data-ttu-id="aec14-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec14-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-121">Not supported.</span></span>    | <span data-ttu-id="aec14-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-122">Not supported.</span></span> |
|<span data-ttu-id="aec14-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="aec14-123">Application</span></span> | <span data-ttu-id="aec14-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="aec14-124">ChannelMessage.Read.All</span></span> | <span data-ttu-id="aec14-125">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="aec14-125">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="aec14-126">示例</span><span class="sxs-lookup"><span data-stu-id="aec14-126">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="aec14-127">跨聊天订阅消息</span><span class="sxs-lookup"><span data-stu-id="aec14-127">Subscribe to messages across chats</span></span>

<span data-ttu-id="aec14-128">若要跨租户中的聊天获取所有消息的更改通知，请订阅 `/chats/getAllMessages`。</span><span class="sxs-lookup"><span data-stu-id="aec14-128">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="aec14-129">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="aec14-129">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="aec14-130">权限</span><span class="sxs-lookup"><span data-stu-id="aec14-130">Permissions</span></span>

|<span data-ttu-id="aec14-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="aec14-131">Permission type</span></span>      | <span data-ttu-id="aec14-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aec14-132">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="aec14-133">支持的版本</span><span class="sxs-lookup"><span data-stu-id="aec14-133">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="aec14-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-134">Delegated (work or school account)</span></span> | <span data-ttu-id="aec14-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-135">Not supported.</span></span> | <span data-ttu-id="aec14-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-136">Not supported.</span></span> |
|<span data-ttu-id="aec14-137">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec14-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-138">Not supported.</span></span>    | <span data-ttu-id="aec14-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-139">Not supported.</span></span> |
|<span data-ttu-id="aec14-140">应用程序</span><span class="sxs-lookup"><span data-stu-id="aec14-140">Application</span></span> | <span data-ttu-id="aec14-141">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="aec14-141">Chat.Read.All</span></span> | <span data-ttu-id="aec14-142">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="aec14-142">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="aec14-143">示例</span><span class="sxs-lookup"><span data-stu-id="aec14-143">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="aec14-144">订阅频道中的消息</span><span class="sxs-lookup"><span data-stu-id="aec14-144">Subscribe to messages in a channel</span></span>

<span data-ttu-id="aec14-145">若要跟踪频道中的消息和回复，可在频道级别创建更改通知订阅。</span><span class="sxs-lookup"><span data-stu-id="aec14-145">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="aec14-146">为此，请订阅 `/teams{id}/channels/{id}/messages`。</span><span class="sxs-lookup"><span data-stu-id="aec14-146">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="aec14-147">此资源支持在 *仅限应用程序模式* 下 [包括通知中的资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="aec14-147">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="aec14-148">频道级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。</span><span class="sxs-lookup"><span data-stu-id="aec14-148">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="aec14-149">权限</span><span class="sxs-lookup"><span data-stu-id="aec14-149">Permissions</span></span>

|<span data-ttu-id="aec14-150">权限类型</span><span class="sxs-lookup"><span data-stu-id="aec14-150">Permission type</span></span>      | <span data-ttu-id="aec14-151">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aec14-151">Permissions (from least to most privileged)</span></span>              |<span data-ttu-id="aec14-152">版本支持</span><span class="sxs-lookup"><span data-stu-id="aec14-152">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:--------------------|
|<span data-ttu-id="aec14-153">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-153">Delegated (work or school account)</span></span> | <span data-ttu-id="aec14-154">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="aec14-154">ChannelMessage.Read.All</span></span> | <span data-ttu-id="aec14-155">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="aec14-155">beta, v1.0</span></span> |
|<span data-ttu-id="aec14-156">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec14-157">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-157">Not supported.</span></span>    | <span data-ttu-id="aec14-158">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-158">Not supported.</span></span> |
|<span data-ttu-id="aec14-159">应用程序</span><span class="sxs-lookup"><span data-stu-id="aec14-159">Application</span></span> | <span data-ttu-id="aec14-160">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="aec14-160">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> | <span data-ttu-id="aec14-161">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="aec14-161">beta, v1.0</span></span> |

><span data-ttu-id="aec14-162">**注意：** ChannelMessage.Read.Group 作为 [资源特定许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)的一部分受支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-162">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="aec14-163">示例 1：订阅频道中的所有消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="aec14-163">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="aec14-164">示例 2：订阅频道中包含特定文本的消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="aec14-164">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="aec14-165">以下请求将向订阅者发送包含 `Hello` 的消息。</span><span class="sxs-lookup"><span data-stu-id="aec14-165">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="aec14-166">示例 3：订阅频道中的消息（和回复），不含资源数据</span><span class="sxs-lookup"><span data-stu-id="aec14-166">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="aec14-167">示例 4：订阅频道中提到特定用户的消息（和回复）</span><span class="sxs-lookup"><span data-stu-id="aec14-167">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="aec14-168">要仅获得提到特定用户的消息，你可以在查询中指定用户的 ID（在此示例中为 `9a6eb4d1-826b-48b1-9627-b50836c8fee9`）。</span><span class="sxs-lookup"><span data-stu-id="aec14-168">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="aec14-169">订阅聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="aec14-169">Subscribe to messages in a chat</span></span>

<span data-ttu-id="aec14-170">若要跟踪聊天中的消息，你可以在聊天级别创建更改通知订阅。</span><span class="sxs-lookup"><span data-stu-id="aec14-170">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="aec14-171">为此，请订阅 `/chats{id}/messages`。</span><span class="sxs-lookup"><span data-stu-id="aec14-171">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="aec14-172">此资源支持在 *仅限应用程序模式* 下 [包括通知中的资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="aec14-172">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="aec14-173">聊天级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。</span><span class="sxs-lookup"><span data-stu-id="aec14-173">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="aec14-174">**注意。**</span><span class="sxs-lookup"><span data-stu-id="aec14-174">**Note.**</span></span> <span data-ttu-id="aec14-175">订阅聊天中的消息目前在预览中。</span><span class="sxs-lookup"><span data-stu-id="aec14-175">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="aec14-176">权限</span><span class="sxs-lookup"><span data-stu-id="aec14-176">Permissions</span></span>

|<span data-ttu-id="aec14-177">权限类型</span><span class="sxs-lookup"><span data-stu-id="aec14-177">Permission type</span></span>      | <span data-ttu-id="aec14-178">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aec14-178">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="aec14-179">版本支持</span><span class="sxs-lookup"><span data-stu-id="aec14-179">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:---------------------|
|<span data-ttu-id="aec14-180">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-180">Delegated (work or school account)</span></span> | <span data-ttu-id="aec14-181">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="aec14-181">Chat.Read</span></span> | <span data-ttu-id="aec14-182">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="aec14-182">beta, v1.0</span></span> |
|<span data-ttu-id="aec14-183">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aec14-183">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec14-184">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-184">Not supported.</span></span>    | <span data-ttu-id="aec14-185">不支持。</span><span class="sxs-lookup"><span data-stu-id="aec14-185">Not supported.</span></span> |
|<span data-ttu-id="aec14-186">应用程序</span><span class="sxs-lookup"><span data-stu-id="aec14-186">Application</span></span> | <span data-ttu-id="aec14-187">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="aec14-187">Chat.Read.All</span></span> | <span data-ttu-id="aec14-188">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="aec14-188">beta, v1.0</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="aec14-189">示例 1：订阅聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="aec14-189">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="aec14-190">示例 2：订阅聊天中包含特定文本的消息</span><span class="sxs-lookup"><span data-stu-id="aec14-190">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="aec14-191">以下请求将向订阅者发送包含 `Hello` 的消息。</span><span class="sxs-lookup"><span data-stu-id="aec14-191">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="aec14-192">示例 3：订阅聊天中的消息（和回复），不含资源数据</span><span class="sxs-lookup"><span data-stu-id="aec14-192">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="aec14-193">示例 4：订阅聊天中提到特定用户的消息</span><span class="sxs-lookup"><span data-stu-id="aec14-193">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="aec14-194">要仅获得提到特定用户的消息，你可以在查询中指定用户的 ID（在此示例中为 `9a6eb4d1-826b-48b1-9627-b50836c8fee9`）。</span><span class="sxs-lookup"><span data-stu-id="aec14-194">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="notification-payloads"></a><span data-ttu-id="aec14-195">通知负载</span><span class="sxs-lookup"><span data-stu-id="aec14-195">Notification payloads</span></span>

<span data-ttu-id="aec14-196">根据你的订阅，你可以获取包含或不含资源数据的通知。</span><span class="sxs-lookup"><span data-stu-id="aec14-196">Depending on your subscription, you can either get the notification with resource data, or without it.</span></span> <span data-ttu-id="aec14-197">通过订阅资源数据，你将在收到通知的同时获得消息负载，而无需回调并获取内容。</span><span class="sxs-lookup"><span data-stu-id="aec14-197">Subscribing with resource data allows you to get the message payload along with the notification, removing the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="aec14-198">包含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="aec14-198">Notifications with resource data</span></span>

<span data-ttu-id="aec14-199">对于包含资源数据的通知，负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="aec14-199">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="aec14-200">此负载适用于在聊天中发送的消息。</span><span class="sxs-lookup"><span data-stu-id="aec14-200">This payload is for a message sent in a chat.</span></span>

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

<span data-ttu-id="aec14-201">有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="aec14-201">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="aec14-202">解密的通知负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="aec14-202">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="aec14-203">该负载符合 [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="aec14-203">The payload conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="aec14-204">该负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="aec14-204">The payload is similar to that returned by GET operations.</span></span>

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

### <a name="notifications-without-resource-data"></a><span data-ttu-id="aec14-205">不含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="aec14-205">Notifications without resource data</span></span>

<span data-ttu-id="aec14-206">不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取消息内容。</span><span class="sxs-lookup"><span data-stu-id="aec14-206">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="aec14-207">订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。</span><span class="sxs-lookup"><span data-stu-id="aec14-207">Subscriptions for notifications without resource data do not require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="aec14-208">该负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="aec14-208">The payload looks like the following.</span></span> <span data-ttu-id="aec14-209">此负载适用于在频道中发送的消息。</span><span class="sxs-lookup"><span data-stu-id="aec14-209">This payload is for a message sent in a channel.</span></span>

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

<span data-ttu-id="aec14-210">**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息负载。</span><span class="sxs-lookup"><span data-stu-id="aec14-210">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="aec14-211">GET 调用将始终返回消息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="aec14-211">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="aec14-212">如果在发送通知和检索消息之间更改了消息，则该操作将返回更新的消息。</span><span class="sxs-lookup"><span data-stu-id="aec14-212">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="aec14-213">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aec14-213">See also</span></span>
- [<span data-ttu-id="aec14-214">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="aec14-214">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="aec14-215">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="aec14-215">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
