---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 资源的数据发生更改时接收通知。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 550cec423d03c2fc1bf4e589675dcfeb126c39d8
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331274"
---
# <a name="create-subscription"></a><span data-ttu-id="292b6-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="292b6-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="292b6-104">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收通知。</span><span class="sxs-lookup"><span data-stu-id="292b6-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="292b6-105">权限</span><span class="sxs-lookup"><span data-stu-id="292b6-105">Permissions</span></span>

<span data-ttu-id="292b6-106">创建订阅需要对资源具有读取权限。</span><span class="sxs-lookup"><span data-stu-id="292b6-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="292b6-107">例如，若要获取有关邮件的通知，您的应用程序需要具有邮件读取权限。</span><span class="sxs-lookup"><span data-stu-id="292b6-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="292b6-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="292b6-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="292b6-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="292b6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="292b6-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="292b6-110">Supported resource</span></span> | <span data-ttu-id="292b6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="292b6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="292b6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="292b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="292b6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="292b6-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="292b6-114">[了 chatmessage](../resources/chatmessage.md) （/teams/{id}/channels/{id}/messages）</span><span class="sxs-lookup"><span data-stu-id="292b6-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="292b6-115">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-115">Not supported</span></span> | <span data-ttu-id="292b6-116">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-116">Not supported</span></span> | <span data-ttu-id="292b6-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="292b6-118">[了 chatmessage](../resources/chatmessage.md) （/teams/allMessages--组织中的所有频道邮件）</span><span class="sxs-lookup"><span data-stu-id="292b6-118">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="292b6-119">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-119">Not supported</span></span> | <span data-ttu-id="292b6-120">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-120">Not supported</span></span> | <span data-ttu-id="292b6-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-121">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="292b6-122">[了 chatmessage](../resources/chatmessage.md) （/chats/{id}/messages）</span><span class="sxs-lookup"><span data-stu-id="292b6-122">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="292b6-123">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-123">Not supported</span></span> | <span data-ttu-id="292b6-124">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-124">Not supported</span></span> | <span data-ttu-id="292b6-125">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-125">Chat.Read.All</span></span>  |
|<span data-ttu-id="292b6-126">[了 chatmessage](../resources/chatmessage.md) （/chats/allMessages--组织中的所有聊天邮件）</span><span class="sxs-lookup"><span data-stu-id="292b6-126">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="292b6-127">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-127">Not supported</span></span> | <span data-ttu-id="292b6-128">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-128">Not supported</span></span> | <span data-ttu-id="292b6-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-129">Chat.Read.All</span></span>  |
|[<span data-ttu-id="292b6-130">联系人</span><span class="sxs-lookup"><span data-stu-id="292b6-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="292b6-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-131">Contacts.Read</span></span> | <span data-ttu-id="292b6-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-132">Contacts.Read</span></span> | <span data-ttu-id="292b6-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-133">Contacts.Read</span></span> |
|<span data-ttu-id="292b6-134">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="292b6-134">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="292b6-135">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-135">Not supported</span></span> | <span data-ttu-id="292b6-136">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="292b6-136">Files.ReadWrite</span></span> | <span data-ttu-id="292b6-137">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-137">Not supported</span></span> |
|<span data-ttu-id="292b6-138">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="292b6-138">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="292b6-139">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292b6-139">Files.ReadWrite.All</span></span> | <span data-ttu-id="292b6-140">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-140">Not supported</span></span> | <span data-ttu-id="292b6-141">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292b6-141">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="292b6-142">事件</span><span class="sxs-lookup"><span data-stu-id="292b6-142">event</span></span>](../resources/event.md) | <span data-ttu-id="292b6-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-143">Calendars.Read</span></span> | <span data-ttu-id="292b6-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-144">Calendars.Read</span></span> | <span data-ttu-id="292b6-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-145">Calendars.Read</span></span> |
|[<span data-ttu-id="292b6-146">组</span><span class="sxs-lookup"><span data-stu-id="292b6-146">group</span></span>](../resources/group.md) | <span data-ttu-id="292b6-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-147">Group.Read.All</span></span> | <span data-ttu-id="292b6-148">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-148">Not supported</span></span> | <span data-ttu-id="292b6-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-149">Group.Read.All</span></span> |
|[<span data-ttu-id="292b6-150">组对话</span><span class="sxs-lookup"><span data-stu-id="292b6-150">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="292b6-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-151">Group.Read.All</span></span> | <span data-ttu-id="292b6-152">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-152">Not supported</span></span> | <span data-ttu-id="292b6-153">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-153">Not supported</span></span> |
|[<span data-ttu-id="292b6-154">list</span><span class="sxs-lookup"><span data-stu-id="292b6-154">list</span></span>](../resources/list.md) | <span data-ttu-id="292b6-155">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292b6-155">Sites.ReadWrite.All</span></span> | <span data-ttu-id="292b6-156">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-156">Not supported</span></span> | <span data-ttu-id="292b6-157">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292b6-157">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="292b6-158">邮件</span><span class="sxs-lookup"><span data-stu-id="292b6-158">message</span></span>](../resources/message.md) | <span data-ttu-id="292b6-159">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-159">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="292b6-160">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-160">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="292b6-161">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="292b6-161">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="292b6-162">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="292b6-162">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="292b6-163">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292b6-163">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="292b6-164">不支持</span><span class="sxs-lookup"><span data-stu-id="292b6-164">Not supported</span></span> | <span data-ttu-id="292b6-165">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292b6-165">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="292b6-166">用户</span><span class="sxs-lookup"><span data-stu-id="292b6-166">user</span></span>](../resources/user.md) | <span data-ttu-id="292b6-167">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-167">User.Read.All</span></span> | <span data-ttu-id="292b6-168">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-168">User.Read.All</span></span> | <span data-ttu-id="292b6-169">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="292b6-169">User.Read.All</span></span> |

### <a name="chatmessage-microsoft-teams"></a><span data-ttu-id="292b6-170">了 chatmessage （Microsoft 团队）</span><span class="sxs-lookup"><span data-stu-id="292b6-170">chatMessage (Microsoft Teams)</span></span>

<span data-ttu-id="292b6-171">**了 chatmessage**订阅需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="292b6-171">**chatMessage** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="292b6-172">如果未指定[encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="292b6-172">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="292b6-173">在创建**了 chatmessage**订阅之前，您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="292b6-173">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="292b6-174">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="292b6-174">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="292b6-175">**注意：** `/teams/allMessages`和`/chats/allMessages`当前处于预览阶段。</span><span class="sxs-lookup"><span data-stu-id="292b6-175">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="292b6-176">在预览过程中，可以在不付费的情况下使用此 API，这取决于[Microsoft Api 使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context)。</span><span class="sxs-lookup"><span data-stu-id="292b6-176">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="292b6-177">但是，使用 API 的应用程序的用户可能需要订阅特定 Microsoft 365 产品。</span><span class="sxs-lookup"><span data-stu-id="292b6-177">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="292b6-178">在正式发行时，Microsoft 可能会要求您或您的客户根据通过 API 访问的数据量支付额外费用。</span><span class="sxs-lookup"><span data-stu-id="292b6-178">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem-onedrive"></a><span data-ttu-id="292b6-179">driveItem （OneDrive）</span><span class="sxs-lookup"><span data-stu-id="292b6-179">driveItem (OneDrive)</span></span>

<span data-ttu-id="292b6-180">对 OneDrive 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="292b6-180">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="292b6-181">这些限制适用于创建和管理（获取、更新和删除）订阅。</span><span class="sxs-lookup"><span data-stu-id="292b6-181">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="292b6-182">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="292b6-182">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="292b6-183">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="292b6-183">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="292b6-184">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送通知。</span><span class="sxs-lookup"><span data-stu-id="292b6-184">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="292b6-185">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="292b6-185">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message-outlook"></a><span data-ttu-id="292b6-186">联系人、事件和邮件（Outlook）</span><span class="sxs-lookup"><span data-stu-id="292b6-186">contact, event, and message (Outlook)</span></span>

<span data-ttu-id="292b6-187">对 Outlook 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="292b6-187">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="292b6-188">这些限制适用于创建和管理（获取、更新和删除）订阅。</span><span class="sxs-lookup"><span data-stu-id="292b6-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="292b6-189">委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="292b6-189">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="292b6-190">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="292b6-190">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="292b6-191">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="292b6-191">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="292b6-192">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="292b6-192">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="292b6-193">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="292b6-193">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="292b6-194">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="292b6-194">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="292b6-195">请求标头</span><span class="sxs-lookup"><span data-stu-id="292b6-195">Request headers</span></span>

| <span data-ttu-id="292b6-196">名称</span><span class="sxs-lookup"><span data-stu-id="292b6-196">Name</span></span>       | <span data-ttu-id="292b6-197">类型</span><span class="sxs-lookup"><span data-stu-id="292b6-197">Type</span></span> | <span data-ttu-id="292b6-198">说明</span><span class="sxs-lookup"><span data-stu-id="292b6-198">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="292b6-199">Authorization</span><span class="sxs-lookup"><span data-stu-id="292b6-199">Authorization</span></span>  | <span data-ttu-id="292b6-200">string</span><span class="sxs-lookup"><span data-stu-id="292b6-200">string</span></span>  | <span data-ttu-id="292b6-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="292b6-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="292b6-203">响应</span><span class="sxs-lookup"><span data-stu-id="292b6-203">Response</span></span>

<span data-ttu-id="292b6-204">如果成功，此方法在响应`201 Created`正文中返回响应代码和[订阅](../resources/subscription.md)对象。</span><span class="sxs-lookup"><span data-stu-id="292b6-204">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="292b6-205">示例</span><span class="sxs-lookup"><span data-stu-id="292b6-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="292b6-206">请求</span><span class="sxs-lookup"><span data-stu-id="292b6-206">Request</span></span>

<span data-ttu-id="292b6-207">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="292b6-207">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="292b6-208">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="292b6-208">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="292b6-209">此请求创建一个订阅，用于通知当前登录用户接收到的新邮件。</span><span class="sxs-lookup"><span data-stu-id="292b6-209">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="292b6-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="292b6-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="292b6-211">C#</span><span class="sxs-lookup"><span data-stu-id="292b6-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="292b6-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="292b6-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="292b6-213">Objective-C</span><span class="sxs-lookup"><span data-stu-id="292b6-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="292b6-214">以下是 resource 属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="292b6-214">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="292b6-215">资源类型</span><span class="sxs-lookup"><span data-stu-id="292b6-215">Resource type</span></span> | <span data-ttu-id="292b6-216">示例</span><span class="sxs-lookup"><span data-stu-id="292b6-216">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="292b6-217">邮件</span><span class="sxs-lookup"><span data-stu-id="292b6-217">Mail</span></span>|<span data-ttu-id="292b6-218">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="292b6-218">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="292b6-219">me/messages</span><span class="sxs-lookup"><span data-stu-id="292b6-219">me/messages</span></span>|
|<span data-ttu-id="292b6-220">联系人</span><span class="sxs-lookup"><span data-stu-id="292b6-220">Contacts</span></span>|<span data-ttu-id="292b6-221">me/contacts</span><span class="sxs-lookup"><span data-stu-id="292b6-221">me/contacts</span></span>|
|<span data-ttu-id="292b6-222">日历</span><span class="sxs-lookup"><span data-stu-id="292b6-222">Calendars</span></span>|<span data-ttu-id="292b6-223">me/events</span><span class="sxs-lookup"><span data-stu-id="292b6-223">me/events</span></span>|
|<span data-ttu-id="292b6-224">用户</span><span class="sxs-lookup"><span data-stu-id="292b6-224">Users</span></span>|<span data-ttu-id="292b6-225">users</span><span class="sxs-lookup"><span data-stu-id="292b6-225">users</span></span>|
|<span data-ttu-id="292b6-226">组</span><span class="sxs-lookup"><span data-stu-id="292b6-226">Groups</span></span>|<span data-ttu-id="292b6-227">groups</span><span class="sxs-lookup"><span data-stu-id="292b6-227">groups</span></span>|
|<span data-ttu-id="292b6-228">对话</span><span class="sxs-lookup"><span data-stu-id="292b6-228">Conversations</span></span>|<span data-ttu-id="292b6-229">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="292b6-229">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="292b6-230">驱动器</span><span class="sxs-lookup"><span data-stu-id="292b6-230">Drives</span></span>|<span data-ttu-id="292b6-231">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="292b6-231">me/drive/root</span></span>|
|<span data-ttu-id="292b6-232">列表</span><span class="sxs-lookup"><span data-stu-id="292b6-232">List</span></span>|<span data-ttu-id="292b6-233">site/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="292b6-233">site/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="292b6-234">安全警报</span><span class="sxs-lookup"><span data-stu-id="292b6-234">Security alert</span></span>|<span data-ttu-id="292b6-235">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="292b6-235">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="292b6-236">响应</span><span class="sxs-lookup"><span data-stu-id="292b6-236">Response</span></span>

<span data-ttu-id="292b6-237">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="292b6-237">The following example shows the response.</span></span> 

><span data-ttu-id="292b6-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="292b6-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="292b6-240">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="292b6-240">Notification endpoint validation</span></span>

<span data-ttu-id="292b6-241">订阅通知终结点（在**notificationUrl**属性中指定）必须能够响应验证请求，如[设置用户数据中的更改通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="292b6-241">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="292b6-242">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="292b6-242">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
