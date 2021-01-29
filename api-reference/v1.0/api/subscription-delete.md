---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b4b05d659453ef0867d60f3d43d137f4b697874
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034071"
---
# <a name="delete-subscription"></a><span data-ttu-id="e4a36-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="e4a36-103">Delete subscription</span></span>

<span data-ttu-id="e4a36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4a36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4a36-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="e4a36-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a36-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4a36-106">Permissions</span></span>

<span data-ttu-id="e4a36-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="e4a36-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e4a36-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4a36-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4a36-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="e4a36-109">Supported resource</span></span> | <span data-ttu-id="e4a36-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a36-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a36-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a36-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4a36-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e4a36-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="e4a36-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="e4a36-114">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-114">Not supported</span></span> | <span data-ttu-id="e4a36-115">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-115">Not supported</span></span> | <span data-ttu-id="e4a36-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="e4a36-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e4a36-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="e4a36-118">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-118">Not supported</span></span> | <span data-ttu-id="e4a36-119">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-119">Not supported</span></span> |  <span data-ttu-id="e4a36-120">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e4a36-121">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="e4a36-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="e4a36-122">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-122">Not supported</span></span> | <span data-ttu-id="e4a36-123">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-123">Not supported</span></span> | <span data-ttu-id="e4a36-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e4a36-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="e4a36-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="e4a36-126">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-126">Not supported</span></span> | <span data-ttu-id="e4a36-127">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-127">Not supported</span></span> | <span data-ttu-id="e4a36-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="e4a36-129">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="e4a36-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="e4a36-130">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-130">Not supported</span></span> | <span data-ttu-id="e4a36-131">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-131">Not supported</span></span> | <span data-ttu-id="e4a36-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="e4a36-133">contact</span><span class="sxs-lookup"><span data-stu-id="e4a36-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e4a36-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-134">Contacts.Read</span></span> | <span data-ttu-id="e4a36-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-135">Contacts.Read</span></span> | <span data-ttu-id="e4a36-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-136">Contacts.Read</span></span> |
|<span data-ttu-id="e4a36-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="e4a36-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e4a36-138">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-138">Not supported</span></span> | <span data-ttu-id="e4a36-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4a36-139">Files.ReadWrite</span></span> | <span data-ttu-id="e4a36-140">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-140">Not supported</span></span> |
|<span data-ttu-id="e4a36-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e4a36-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e4a36-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="e4a36-143">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-143">Not supported</span></span> | <span data-ttu-id="e4a36-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e4a36-145">事件</span><span class="sxs-lookup"><span data-stu-id="e4a36-145">event</span></span>](../resources/event.md) | <span data-ttu-id="e4a36-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-146">Calendars.Read</span></span> | <span data-ttu-id="e4a36-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-147">Calendars.Read</span></span> | <span data-ttu-id="e4a36-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-148">Calendars.Read</span></span> |
|[<span data-ttu-id="e4a36-149">组</span><span class="sxs-lookup"><span data-stu-id="e4a36-149">group</span></span>](../resources/group.md) | <span data-ttu-id="e4a36-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-150">Group.Read.All</span></span> | <span data-ttu-id="e4a36-151">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-151">Not supported</span></span> | <span data-ttu-id="e4a36-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-152">Group.Read.All</span></span> |
|[<span data-ttu-id="e4a36-153">组对话</span><span class="sxs-lookup"><span data-stu-id="e4a36-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e4a36-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-154">Group.Read.All</span></span> | <span data-ttu-id="e4a36-155">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-155">Not supported</span></span> | <span data-ttu-id="e4a36-156">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-156">Not supported</span></span> |
|[<span data-ttu-id="e4a36-157">列表</span><span class="sxs-lookup"><span data-stu-id="e4a36-157">list</span></span>](../resources/list.md) | <span data-ttu-id="e4a36-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e4a36-159">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-159">Not supported</span></span> | <span data-ttu-id="e4a36-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e4a36-161">邮件</span><span class="sxs-lookup"><span data-stu-id="e4a36-161">message</span></span>](../resources/message.md) | <span data-ttu-id="e4a36-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e4a36-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e4a36-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e4a36-164">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="e4a36-165">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="e4a36-165">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="e4a36-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e4a36-167">不支持</span><span class="sxs-lookup"><span data-stu-id="e4a36-167">Not supported</span></span> | <span data-ttu-id="e4a36-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="e4a36-169">用户</span><span class="sxs-lookup"><span data-stu-id="e4a36-169">user</span></span>](../resources/user.md) | <span data-ttu-id="e4a36-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-170">User.Read.All</span></span> | <span data-ttu-id="e4a36-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-171">User.Read.All</span></span> | <span data-ttu-id="e4a36-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a36-172">User.Read.All</span></span> |

> <span data-ttu-id="e4a36-173">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="e4a36-173">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="e4a36-174">driveItem</span><span class="sxs-lookup"><span data-stu-id="e4a36-174">driveItem</span></span>

<span data-ttu-id="e4a36-175">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="e4a36-175">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="e4a36-176">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="e4a36-176">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="e4a36-177">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="e4a36-177">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e4a36-178">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="e4a36-178">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e4a36-179">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="e4a36-179">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="e4a36-180">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="e4a36-180">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="e4a36-181">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="e4a36-181">contact, event, and message</span></span>

<span data-ttu-id="e4a36-182">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="e4a36-182">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="e4a36-183">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="e4a36-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="e4a36-184">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="e4a36-184">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e4a36-185">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="e4a36-185">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="e4a36-186">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="e4a36-186">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e4a36-187">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="e4a36-187">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e4a36-188">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="e4a36-188">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="e4a36-189">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4a36-189">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="e4a36-190">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4a36-190">Request headers</span></span>

| <span data-ttu-id="e4a36-191">名称</span><span class="sxs-lookup"><span data-stu-id="e4a36-191">Name</span></span>       | <span data-ttu-id="e4a36-192">类型</span><span class="sxs-lookup"><span data-stu-id="e4a36-192">Type</span></span> | <span data-ttu-id="e4a36-193">说明</span><span class="sxs-lookup"><span data-stu-id="e4a36-193">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e4a36-194">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4a36-194">Authorization</span></span>  | <span data-ttu-id="e4a36-195">string</span><span class="sxs-lookup"><span data-stu-id="e4a36-195">string</span></span>  | <span data-ttu-id="e4a36-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4a36-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4a36-198">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4a36-198">Request body</span></span>

<span data-ttu-id="e4a36-199">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4a36-199">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4a36-200">响应</span><span class="sxs-lookup"><span data-stu-id="e4a36-200">Response</span></span>

<span data-ttu-id="e4a36-201">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e4a36-201">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="e4a36-202">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="e4a36-202">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e4a36-203">示例</span><span class="sxs-lookup"><span data-stu-id="e4a36-203">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e4a36-204">请求</span><span class="sxs-lookup"><span data-stu-id="e4a36-204">Request</span></span>

<span data-ttu-id="e4a36-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4a36-205">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4a36-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a36-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="e4a36-207">C#</span><span class="sxs-lookup"><span data-stu-id="e4a36-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4a36-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4a36-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4a36-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4a36-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4a36-210">Java</span><span class="sxs-lookup"><span data-stu-id="e4a36-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4a36-211">响应</span><span class="sxs-lookup"><span data-stu-id="e4a36-211">Response</span></span>

<span data-ttu-id="e4a36-212">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e4a36-212">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

