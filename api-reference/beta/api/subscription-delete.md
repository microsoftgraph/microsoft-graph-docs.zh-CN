---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fbf44321322d51bc237715f7b4555a68655ee10
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848687"
---
# <a name="delete-subscription"></a><span data-ttu-id="34a73-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="34a73-103">Delete subscription</span></span>

<span data-ttu-id="34a73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34a73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34a73-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="34a73-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="34a73-106">权限</span><span class="sxs-lookup"><span data-stu-id="34a73-106">Permissions</span></span>

<span data-ttu-id="34a73-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="34a73-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="34a73-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34a73-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34a73-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="34a73-109">Supported resource</span></span> | <span data-ttu-id="34a73-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34a73-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34a73-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34a73-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34a73-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="34a73-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="34a73-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="34a73-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="34a73-114">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-114">Not supported</span></span> | <span data-ttu-id="34a73-115">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-115">Not supported</span></span> | <span data-ttu-id="34a73-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="34a73-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="34a73-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="34a73-118">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a73-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="34a73-119">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-119">Not supported</span></span> | <span data-ttu-id="34a73-120">ChannelMessage \*、ChannelMessage \*。</span><span class="sxs-lookup"><span data-stu-id="34a73-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="34a73-121">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="34a73-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="34a73-122">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-122">Not supported</span></span> | <span data-ttu-id="34a73-123">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-123">Not supported</span></span> | <span data-ttu-id="34a73-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="34a73-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="34a73-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="34a73-126">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a73-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="34a73-127">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-127">Not supported</span></span> | <span data-ttu-id="34a73-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="34a73-129">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="34a73-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="34a73-130">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-130">Not supported</span></span> | <span data-ttu-id="34a73-131">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-131">Not supported</span></span> | <span data-ttu-id="34a73-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="34a73-133">contact</span><span class="sxs-lookup"><span data-stu-id="34a73-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="34a73-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-134">Contacts.Read</span></span> | <span data-ttu-id="34a73-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-135">Contacts.Read</span></span> | <span data-ttu-id="34a73-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-136">Contacts.Read</span></span> |
|<span data-ttu-id="34a73-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="34a73-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="34a73-138">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-138">Not supported</span></span> | <span data-ttu-id="34a73-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a73-139">Files.ReadWrite</span></span> | <span data-ttu-id="34a73-140">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-140">Not supported</span></span> |
|<span data-ttu-id="34a73-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="34a73-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="34a73-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a73-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="34a73-143">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-143">Not supported</span></span> | <span data-ttu-id="34a73-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a73-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="34a73-145">事件</span><span class="sxs-lookup"><span data-stu-id="34a73-145">event</span></span>](../resources/event.md) | <span data-ttu-id="34a73-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-146">Calendars.Read</span></span> | <span data-ttu-id="34a73-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-147">Calendars.Read</span></span> | <span data-ttu-id="34a73-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-148">Calendars.Read</span></span> |
|[<span data-ttu-id="34a73-149">组</span><span class="sxs-lookup"><span data-stu-id="34a73-149">group</span></span>](../resources/group.md) | <span data-ttu-id="34a73-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-150">Group.Read.All</span></span> | <span data-ttu-id="34a73-151">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-151">Not supported</span></span> | <span data-ttu-id="34a73-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-152">Group.Read.All</span></span> |
|[<span data-ttu-id="34a73-153">组对话</span><span class="sxs-lookup"><span data-stu-id="34a73-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="34a73-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-154">Group.Read.All</span></span> | <span data-ttu-id="34a73-155">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-155">Not supported</span></span> | <span data-ttu-id="34a73-156">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-156">Not supported</span></span> |
|[<span data-ttu-id="34a73-157">列表</span><span class="sxs-lookup"><span data-stu-id="34a73-157">list</span></span>](../resources/list.md) | <span data-ttu-id="34a73-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a73-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="34a73-159">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-159">Not supported</span></span> | <span data-ttu-id="34a73-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a73-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="34a73-161">邮件</span><span class="sxs-lookup"><span data-stu-id="34a73-161">message</span></span>](../resources/message.md) | <span data-ttu-id="34a73-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="34a73-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="34a73-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="34a73-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="34a73-165">状态</span><span class="sxs-lookup"><span data-stu-id="34a73-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="34a73-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-166">Presence.Read.All</span></span> | <span data-ttu-id="34a73-167">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-167">Not supported</span></span> | <span data-ttu-id="34a73-168">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-168">Not supported</span></span> |
|<span data-ttu-id="34a73-169">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="34a73-169">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="34a73-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a73-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="34a73-171">不支持</span><span class="sxs-lookup"><span data-stu-id="34a73-171">Not supported</span></span> | <span data-ttu-id="34a73-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a73-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="34a73-173">用户</span><span class="sxs-lookup"><span data-stu-id="34a73-173">user</span></span>](../resources/user.md) | <span data-ttu-id="34a73-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-174">User.Read.All</span></span> | <span data-ttu-id="34a73-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-175">User.Read.All</span></span> | <span data-ttu-id="34a73-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a73-176">User.Read.All</span></span> |

> <span data-ttu-id="34a73-177">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="34a73-177">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="34a73-178">chatMessage</span><span class="sxs-lookup"><span data-stu-id="34a73-178">chatMessage</span></span>

<span data-ttu-id="34a73-179">具有委派权限的 **了 chatmessage** 订阅不支持资源数据 ( **includeResourceData** 必须 `false`) ，并且不需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="34a73-179">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="34a73-180">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="34a73-180">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="34a73-181">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="34a73-181">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="34a73-182">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="34a73-182">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="34a73-183">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="34a73-183">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="34a73-184">**注意：** `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="34a73-184">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="34a73-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="34a73-185">driveItem</span></span>

<span data-ttu-id="34a73-186">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="34a73-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="34a73-187">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="34a73-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="34a73-188">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="34a73-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="34a73-189">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="34a73-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="34a73-190">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="34a73-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="34a73-191">无法订阅不是文件夹的“ **驱动器** ”或“ **driveItem** ”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="34a73-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="34a73-192">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="34a73-192">contact, event, and message</span></span>

<span data-ttu-id="34a73-193">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="34a73-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="34a73-194">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="34a73-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="34a73-195">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="34a73-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="34a73-196">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="34a73-196">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="34a73-197">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="34a73-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="34a73-198">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="34a73-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="34a73-199">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="34a73-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="34a73-200">状态</span><span class="sxs-lookup"><span data-stu-id="34a73-200">presence</span></span>

<span data-ttu-id="34a73-201">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="34a73-201">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="34a73-202">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="34a73-202">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="34a73-203">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34a73-203">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="34a73-204">请求标头</span><span class="sxs-lookup"><span data-stu-id="34a73-204">Request headers</span></span>

| <span data-ttu-id="34a73-205">名称</span><span class="sxs-lookup"><span data-stu-id="34a73-205">Name</span></span>       | <span data-ttu-id="34a73-206">类型</span><span class="sxs-lookup"><span data-stu-id="34a73-206">Type</span></span> | <span data-ttu-id="34a73-207">说明</span><span class="sxs-lookup"><span data-stu-id="34a73-207">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34a73-208">Authorization</span><span class="sxs-lookup"><span data-stu-id="34a73-208">Authorization</span></span>  | <span data-ttu-id="34a73-209">string</span><span class="sxs-lookup"><span data-stu-id="34a73-209">string</span></span>  | <span data-ttu-id="34a73-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="34a73-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34a73-212">请求正文</span><span class="sxs-lookup"><span data-stu-id="34a73-212">Request body</span></span>

<span data-ttu-id="34a73-213">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34a73-213">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34a73-214">响应</span><span class="sxs-lookup"><span data-stu-id="34a73-214">Response</span></span>

<span data-ttu-id="34a73-215">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="34a73-215">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="34a73-216">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="34a73-216">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="34a73-217">示例</span><span class="sxs-lookup"><span data-stu-id="34a73-217">Example</span></span>

##### <a name="request"></a><span data-ttu-id="34a73-218">请求</span><span class="sxs-lookup"><span data-stu-id="34a73-218">Request</span></span>

<span data-ttu-id="34a73-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34a73-219">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34a73-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="34a73-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="34a73-221">C#</span><span class="sxs-lookup"><span data-stu-id="34a73-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34a73-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34a73-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34a73-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34a73-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="34a73-224">响应</span><span class="sxs-lookup"><span data-stu-id="34a73-224">Response</span></span>

<span data-ttu-id="34a73-225">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="34a73-225">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


