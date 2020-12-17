---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收更改通知。
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d751cd722bcbf69ac00dae4200424ed9ba0e25f2
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848182"
---
# <a name="create-subscription"></a><span data-ttu-id="ca8f7-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="ca8f7-103">Create subscription</span></span>

<span data-ttu-id="ca8f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca8f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca8f7-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca8f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="ca8f7-106">Permissions</span></span>

 <span data-ttu-id="ca8f7-107">创建订阅需要读取资源范围。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="ca8f7-108">例如，若要获取更改消息通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-108">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="ca8f7-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ca8f7-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca8f7-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="ca8f7-111">Supported resource</span></span> | <span data-ttu-id="ca8f7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca8f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca8f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca8f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca8f7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca8f7-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="ca8f7-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="ca8f7-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="ca8f7-116">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-116">Not supported</span></span> | <span data-ttu-id="ca8f7-117">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-117">Not supported</span></span> | <span data-ttu-id="ca8f7-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="ca8f7-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="ca8f7-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="ca8f7-120">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-120">Not supported</span></span> | <span data-ttu-id="ca8f7-121">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-121">Not supported</span></span> |  <span data-ttu-id="ca8f7-122">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="ca8f7-123">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="ca8f7-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="ca8f7-124">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-124">Not supported</span></span> | <span data-ttu-id="ca8f7-125">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-125">Not supported</span></span> | <span data-ttu-id="ca8f7-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="ca8f7-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="ca8f7-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="ca8f7-128">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-128">Not supported</span></span> | <span data-ttu-id="ca8f7-129">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-129">Not supported</span></span> | <span data-ttu-id="ca8f7-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="ca8f7-131">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="ca8f7-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="ca8f7-132">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-132">Not supported</span></span> | <span data-ttu-id="ca8f7-133">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-133">Not supported</span></span> | <span data-ttu-id="ca8f7-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="ca8f7-135">contact</span><span class="sxs-lookup"><span data-stu-id="ca8f7-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ca8f7-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-136">Contacts.Read</span></span> | <span data-ttu-id="ca8f7-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-137">Contacts.Read</span></span> | <span data-ttu-id="ca8f7-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-138">Contacts.Read</span></span> |
|<span data-ttu-id="ca8f7-139">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="ca8f7-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="ca8f7-140">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-140">Not supported</span></span> | <span data-ttu-id="ca8f7-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8f7-141">Files.ReadWrite</span></span> | <span data-ttu-id="ca8f7-142">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-142">Not supported</span></span> |
|<span data-ttu-id="ca8f7-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="ca8f7-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="ca8f7-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="ca8f7-145">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-145">Not supported</span></span> | <span data-ttu-id="ca8f7-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="ca8f7-147">事件</span><span class="sxs-lookup"><span data-stu-id="ca8f7-147">event</span></span>](../resources/event.md) | <span data-ttu-id="ca8f7-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-148">Calendars.Read</span></span> | <span data-ttu-id="ca8f7-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-149">Calendars.Read</span></span> | <span data-ttu-id="ca8f7-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-150">Calendars.Read</span></span> |
|[<span data-ttu-id="ca8f7-151">组</span><span class="sxs-lookup"><span data-stu-id="ca8f7-151">group</span></span>](../resources/group.md) | <span data-ttu-id="ca8f7-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-152">Group.Read.All</span></span> | <span data-ttu-id="ca8f7-153">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-153">Not supported</span></span> | <span data-ttu-id="ca8f7-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-154">Group.Read.All</span></span> |
|[<span data-ttu-id="ca8f7-155">组对话</span><span class="sxs-lookup"><span data-stu-id="ca8f7-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="ca8f7-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-156">Group.Read.All</span></span> | <span data-ttu-id="ca8f7-157">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-157">Not supported</span></span> | <span data-ttu-id="ca8f7-158">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-158">Not supported</span></span> |
|[<span data-ttu-id="ca8f7-159">列表</span><span class="sxs-lookup"><span data-stu-id="ca8f7-159">list</span></span>](../resources/list.md) | <span data-ttu-id="ca8f7-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="ca8f7-161">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-161">Not supported</span></span> | <span data-ttu-id="ca8f7-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="ca8f7-163">邮件</span><span class="sxs-lookup"><span data-stu-id="ca8f7-163">message</span></span>](../resources/message.md) | <span data-ttu-id="ca8f7-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ca8f7-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ca8f7-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ca8f7-166">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="ca8f7-167">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="ca8f7-167">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="ca8f7-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="ca8f7-169">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8f7-169">Not supported</span></span> | <span data-ttu-id="ca8f7-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="ca8f7-171">用户</span><span class="sxs-lookup"><span data-stu-id="ca8f7-171">user</span></span>](../resources/user.md) | <span data-ttu-id="ca8f7-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-172">User.Read.All</span></span> | <span data-ttu-id="ca8f7-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-173">User.Read.All</span></span> | <span data-ttu-id="ca8f7-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8f7-174">User.Read.All</span></span> |

> <span data-ttu-id="ca8f7-175">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-175">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="ca8f7-176">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ca8f7-176">chatMessage</span></span>

<span data-ttu-id="ca8f7-177">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-177">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="ca8f7-178">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-178">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="ca8f7-179">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-179">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="ca8f7-180">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-180">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="ca8f7-181">**注意：** `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-181">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="ca8f7-182">**注意：** `/chats/getAllMessages` 仅返回租户拥有的聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-182">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="ca8f7-183">如果聊天线程是由租户外部用户发起，则该聊天线程不属于租户，并且不会创建更改通知。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-183">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="ca8f7-184">driveItem</span><span class="sxs-lookup"><span data-stu-id="ca8f7-184">driveItem</span></span>

<span data-ttu-id="ca8f7-185">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-185">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="ca8f7-186">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="ca8f7-187">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-187">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="ca8f7-188">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="ca8f7-189">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="ca8f7-190">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="ca8f7-191">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="ca8f7-191">contact, event, and message</span></span>

<span data-ttu-id="ca8f7-192">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="ca8f7-193">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="ca8f7-194">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="ca8f7-195">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-195">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="ca8f7-196">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="ca8f7-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="ca8f7-197">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="ca8f7-198">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca8f7-199">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca8f7-199">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="ca8f7-200">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca8f7-200">Request headers</span></span>

| <span data-ttu-id="ca8f7-201">名称</span><span class="sxs-lookup"><span data-stu-id="ca8f7-201">Name</span></span>       | <span data-ttu-id="ca8f7-202">类型</span><span class="sxs-lookup"><span data-stu-id="ca8f7-202">Type</span></span> | <span data-ttu-id="ca8f7-203">说明</span><span class="sxs-lookup"><span data-stu-id="ca8f7-203">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca8f7-204">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca8f7-204">Authorization</span></span>  | <span data-ttu-id="ca8f7-205">string</span><span class="sxs-lookup"><span data-stu-id="ca8f7-205">string</span></span>  | <span data-ttu-id="ca8f7-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ca8f7-208">响应</span><span class="sxs-lookup"><span data-stu-id="ca8f7-208">Response</span></span>

<span data-ttu-id="ca8f7-209">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-209">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="ca8f7-210">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-210">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="ca8f7-211">示例</span><span class="sxs-lookup"><span data-stu-id="ca8f7-211">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ca8f7-212">请求</span><span class="sxs-lookup"><span data-stu-id="ca8f7-212">Request</span></span>

<span data-ttu-id="ca8f7-213">下面是在用户收到新邮件时请求发送更改通知的示例。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-213">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca8f7-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8f7-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="ca8f7-215">C#</span><span class="sxs-lookup"><span data-stu-id="ca8f7-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca8f7-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca8f7-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca8f7-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca8f7-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca8f7-218">Java</span><span class="sxs-lookup"><span data-stu-id="ca8f7-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ca8f7-219">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-219">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="ca8f7-220">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-220">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="ca8f7-221">资源示例</span><span class="sxs-lookup"><span data-stu-id="ca8f7-221">Resources examples</span></span>

<span data-ttu-id="ca8f7-222">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="ca8f7-222">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="ca8f7-223">资源类型</span><span class="sxs-lookup"><span data-stu-id="ca8f7-223">Resource type</span></span> | <span data-ttu-id="ca8f7-224">示例</span><span class="sxs-lookup"><span data-stu-id="ca8f7-224">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="ca8f7-225">通话记录</span><span class="sxs-lookup"><span data-stu-id="ca8f7-225">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="ca8f7-226">聊天消息</span><span class="sxs-lookup"><span data-stu-id="ca8f7-226">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ca8f7-227">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="ca8f7-227">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="ca8f7-228">联系人</span><span class="sxs-lookup"><span data-stu-id="ca8f7-228">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="ca8f7-229">对话</span><span class="sxs-lookup"><span data-stu-id="ca8f7-229">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="ca8f7-230">驱动器</span><span class="sxs-lookup"><span data-stu-id="ca8f7-230">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="ca8f7-231">事件</span><span class="sxs-lookup"><span data-stu-id="ca8f7-231">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="ca8f7-232">组</span><span class="sxs-lookup"><span data-stu-id="ca8f7-232">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="ca8f7-233">列表</span><span class="sxs-lookup"><span data-stu-id="ca8f7-233">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="ca8f7-234">邮件</span><span class="sxs-lookup"><span data-stu-id="ca8f7-234">Mail</span></span>](../resources/message.md)|<span data-ttu-id="ca8f7-235">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="ca8f7-235">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="ca8f7-236">用户</span><span class="sxs-lookup"><span data-stu-id="ca8f7-236">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="ca8f7-237">安全警报</span><span class="sxs-lookup"><span data-stu-id="ca8f7-237">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="ca8f7-238">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-238">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="ca8f7-239">响应</span><span class="sxs-lookup"><span data-stu-id="ca8f7-239">Response</span></span>

<span data-ttu-id="ca8f7-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="ca8f7-243">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="ca8f7-243">Notification endpoint validation</span></span>

<span data-ttu-id="ca8f7-244">通知终结点（于 `notificationUrl` 属性中指定）必须能够响应验证请求，如[设置用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-244">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="ca8f7-245">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="ca8f7-245">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

