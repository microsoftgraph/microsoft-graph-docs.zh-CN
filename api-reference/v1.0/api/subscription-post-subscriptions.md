---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收更改通知。
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 95ce278d2f19b30b177912d5b9b799646b6715e7
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034168"
---
# <a name="create-subscription"></a><span data-ttu-id="7c61b-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="7c61b-103">Create subscription</span></span>

<span data-ttu-id="7c61b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c61b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c61b-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="7c61b-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c61b-106">权限</span><span class="sxs-lookup"><span data-stu-id="7c61b-106">Permissions</span></span>

 <span data-ttu-id="7c61b-107">创建订阅需要读取资源范围。</span><span class="sxs-lookup"><span data-stu-id="7c61b-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="7c61b-108">例如，若要获取更改消息通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="7c61b-108">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="7c61b-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="7c61b-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7c61b-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c61b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c61b-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="7c61b-111">Supported resource</span></span> | <span data-ttu-id="7c61b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c61b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7c61b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c61b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c61b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c61b-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="7c61b-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="7c61b-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="7c61b-116">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-116">Not supported</span></span> | <span data-ttu-id="7c61b-117">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-117">Not supported</span></span> | <span data-ttu-id="7c61b-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="7c61b-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7c61b-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="7c61b-120">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-120">Not supported</span></span> | <span data-ttu-id="7c61b-121">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-121">Not supported</span></span> |  <span data-ttu-id="7c61b-122">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7c61b-123">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="7c61b-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="7c61b-124">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-124">Not supported</span></span> | <span data-ttu-id="7c61b-125">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-125">Not supported</span></span> | <span data-ttu-id="7c61b-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7c61b-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7c61b-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="7c61b-128">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-128">Not supported</span></span> | <span data-ttu-id="7c61b-129">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-129">Not supported</span></span> | <span data-ttu-id="7c61b-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="7c61b-131">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="7c61b-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="7c61b-132">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-132">Not supported</span></span> | <span data-ttu-id="7c61b-133">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-133">Not supported</span></span> | <span data-ttu-id="7c61b-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="7c61b-135">contact</span><span class="sxs-lookup"><span data-stu-id="7c61b-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="7c61b-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-136">Contacts.Read</span></span> | <span data-ttu-id="7c61b-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-137">Contacts.Read</span></span> | <span data-ttu-id="7c61b-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-138">Contacts.Read</span></span> |
|<span data-ttu-id="7c61b-139">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="7c61b-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="7c61b-140">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-140">Not supported</span></span> | <span data-ttu-id="7c61b-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c61b-141">Files.ReadWrite</span></span> | <span data-ttu-id="7c61b-142">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-142">Not supported</span></span> |
|<span data-ttu-id="7c61b-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="7c61b-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="7c61b-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="7c61b-145">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-145">Not supported</span></span> | <span data-ttu-id="7c61b-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c61b-147">事件</span><span class="sxs-lookup"><span data-stu-id="7c61b-147">event</span></span>](../resources/event.md) | <span data-ttu-id="7c61b-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-148">Calendars.Read</span></span> | <span data-ttu-id="7c61b-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-149">Calendars.Read</span></span> | <span data-ttu-id="7c61b-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-150">Calendars.Read</span></span> |
|[<span data-ttu-id="7c61b-151">组</span><span class="sxs-lookup"><span data-stu-id="7c61b-151">group</span></span>](../resources/group.md) | <span data-ttu-id="7c61b-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-152">Group.Read.All</span></span> | <span data-ttu-id="7c61b-153">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-153">Not supported</span></span> | <span data-ttu-id="7c61b-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-154">Group.Read.All</span></span> |
|[<span data-ttu-id="7c61b-155">组对话</span><span class="sxs-lookup"><span data-stu-id="7c61b-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="7c61b-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-156">Group.Read.All</span></span> | <span data-ttu-id="7c61b-157">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-157">Not supported</span></span> | <span data-ttu-id="7c61b-158">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-158">Not supported</span></span> |
|[<span data-ttu-id="7c61b-159">列表</span><span class="sxs-lookup"><span data-stu-id="7c61b-159">list</span></span>](../resources/list.md) | <span data-ttu-id="7c61b-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="7c61b-161">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-161">Not supported</span></span> | <span data-ttu-id="7c61b-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c61b-163">邮件</span><span class="sxs-lookup"><span data-stu-id="7c61b-163">message</span></span>](../resources/message.md) | <span data-ttu-id="7c61b-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7c61b-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7c61b-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7c61b-166">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="7c61b-167">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="7c61b-167">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="7c61b-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="7c61b-169">不支持</span><span class="sxs-lookup"><span data-stu-id="7c61b-169">Not supported</span></span> | <span data-ttu-id="7c61b-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c61b-171">用户</span><span class="sxs-lookup"><span data-stu-id="7c61b-171">user</span></span>](../resources/user.md) | <span data-ttu-id="7c61b-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-172">User.Read.All</span></span> | <span data-ttu-id="7c61b-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-173">User.Read.All</span></span> | <span data-ttu-id="7c61b-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c61b-174">User.Read.All</span></span> |

> <span data-ttu-id="7c61b-175">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="7c61b-175">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="7c61b-176">driveItem</span><span class="sxs-lookup"><span data-stu-id="7c61b-176">driveItem</span></span>

<span data-ttu-id="7c61b-177">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="7c61b-177">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="7c61b-178">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="7c61b-178">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="7c61b-179">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="7c61b-179">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="7c61b-180">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="7c61b-180">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="7c61b-181">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="7c61b-181">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="7c61b-182">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="7c61b-182">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="7c61b-183">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="7c61b-183">contact, event, and message</span></span>

<span data-ttu-id="7c61b-184">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="7c61b-184">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="7c61b-185">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="7c61b-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="7c61b-186">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="7c61b-186">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="7c61b-187">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="7c61b-187">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="7c61b-188">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="7c61b-188">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="7c61b-189">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="7c61b-189">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="7c61b-190">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="7c61b-190">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c61b-191">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c61b-191">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="7c61b-192">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c61b-192">Request headers</span></span>

| <span data-ttu-id="7c61b-193">名称</span><span class="sxs-lookup"><span data-stu-id="7c61b-193">Name</span></span>       | <span data-ttu-id="7c61b-194">类型</span><span class="sxs-lookup"><span data-stu-id="7c61b-194">Type</span></span> | <span data-ttu-id="7c61b-195">说明</span><span class="sxs-lookup"><span data-stu-id="7c61b-195">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7c61b-196">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c61b-196">Authorization</span></span>  | <span data-ttu-id="7c61b-197">string</span><span class="sxs-lookup"><span data-stu-id="7c61b-197">string</span></span>  | <span data-ttu-id="7c61b-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c61b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7c61b-200">响应</span><span class="sxs-lookup"><span data-stu-id="7c61b-200">Response</span></span>

<span data-ttu-id="7c61b-201">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c61b-201">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="7c61b-202">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="7c61b-202">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="7c61b-203">示例</span><span class="sxs-lookup"><span data-stu-id="7c61b-203">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7c61b-204">请求</span><span class="sxs-lookup"><span data-stu-id="7c61b-204">Request</span></span>

<span data-ttu-id="7c61b-205">下面是在用户收到新邮件时请求发送更改通知的示例。</span><span class="sxs-lookup"><span data-stu-id="7c61b-205">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c61b-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c61b-206">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7c61b-207">C#</span><span class="sxs-lookup"><span data-stu-id="7c61b-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c61b-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c61b-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c61b-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c61b-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c61b-210">Java</span><span class="sxs-lookup"><span data-stu-id="7c61b-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="7c61b-211">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c61b-211">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="7c61b-212">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="7c61b-212">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="7c61b-213">资源示例</span><span class="sxs-lookup"><span data-stu-id="7c61b-213">Resources examples</span></span>

<span data-ttu-id="7c61b-214">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="7c61b-214">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="7c61b-215">资源类型</span><span class="sxs-lookup"><span data-stu-id="7c61b-215">Resource type</span></span> | <span data-ttu-id="7c61b-216">示例</span><span class="sxs-lookup"><span data-stu-id="7c61b-216">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="7c61b-217">通话记录</span><span class="sxs-lookup"><span data-stu-id="7c61b-217">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="7c61b-218">聊天消息</span><span class="sxs-lookup"><span data-stu-id="7c61b-218">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7c61b-219">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="7c61b-219">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="7c61b-220">联系人</span><span class="sxs-lookup"><span data-stu-id="7c61b-220">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="7c61b-221">对话</span><span class="sxs-lookup"><span data-stu-id="7c61b-221">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="7c61b-222">驱动器</span><span class="sxs-lookup"><span data-stu-id="7c61b-222">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="7c61b-223">事件</span><span class="sxs-lookup"><span data-stu-id="7c61b-223">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="7c61b-224">组</span><span class="sxs-lookup"><span data-stu-id="7c61b-224">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="7c61b-225">列表</span><span class="sxs-lookup"><span data-stu-id="7c61b-225">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="7c61b-226">邮件</span><span class="sxs-lookup"><span data-stu-id="7c61b-226">Mail</span></span>](../resources/message.md)|<span data-ttu-id="7c61b-227">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="7c61b-227">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="7c61b-228">用户</span><span class="sxs-lookup"><span data-stu-id="7c61b-228">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="7c61b-229">安全警报</span><span class="sxs-lookup"><span data-stu-id="7c61b-229">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="7c61b-230">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="7c61b-230">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="7c61b-231">响应</span><span class="sxs-lookup"><span data-stu-id="7c61b-231">Response</span></span>

<span data-ttu-id="7c61b-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c61b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="7c61b-235">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="7c61b-235">Notification endpoint validation</span></span>

<span data-ttu-id="7c61b-236">通知终结点（于 `notificationUrl` 属性中指定）必须能够响应验证请求，如[设置用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="7c61b-236">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="7c61b-237">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="7c61b-237">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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

