---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 22855084a97d4c45199766b1928be04e2318148e
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092419"
---
# <a name="update-subscription"></a><span data-ttu-id="781eb-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="781eb-103">Update subscription</span></span>

<span data-ttu-id="781eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="781eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="781eb-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="781eb-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="781eb-106">"权限" [部分](#permissions) 中的表列出了支持订阅更改通知的资源。</span><span class="sxs-lookup"><span data-stu-id="781eb-106">The table in the [Permissions](#permissions) section lists tje resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="781eb-107">订阅在时间长度因资源类型而异后过期。</span><span class="sxs-lookup"><span data-stu-id="781eb-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="781eb-108">为了避免缺少更改通知，应用应在到期日期之前很好地续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="781eb-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="781eb-109">请参阅 [订阅](../resources/subscription.md) ，了解每种资源类型的订阅的最大长度。</span><span class="sxs-lookup"><span data-stu-id="781eb-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="781eb-110">权限</span><span class="sxs-lookup"><span data-stu-id="781eb-110">Permissions</span></span>

<span data-ttu-id="781eb-111">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="781eb-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="781eb-112">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请搜索"权限"中的以下 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="781eb-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="781eb-113">支持的资源</span><span class="sxs-lookup"><span data-stu-id="781eb-113">Supported resource</span></span> | <span data-ttu-id="781eb-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="781eb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="781eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="781eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="781eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="781eb-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="781eb-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="781eb-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="781eb-118">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-118">Not supported</span></span> | <span data-ttu-id="781eb-119">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-119">Not supported</span></span> | <span data-ttu-id="781eb-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="781eb-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="781eb-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="781eb-122">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-122">Not supported</span></span> | <span data-ttu-id="781eb-123">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-123">Not supported</span></span> |  <span data-ttu-id="781eb-124">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="781eb-125">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="781eb-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="781eb-126">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-126">Not supported</span></span> | <span data-ttu-id="781eb-127">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-127">Not supported</span></span> | <span data-ttu-id="781eb-128">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-128">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="781eb-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="781eb-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="781eb-130">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-130">Not supported</span></span> | <span data-ttu-id="781eb-131">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-131">Not supported</span></span> | <span data-ttu-id="781eb-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-132">Chat.Read.All</span></span>  |
|<span data-ttu-id="781eb-133">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="781eb-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="781eb-134">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-134">Not supported</span></span> | <span data-ttu-id="781eb-135">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-135">Not supported</span></span> | <span data-ttu-id="781eb-136">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-136">Chat.Read.All</span></span>  |
|[<span data-ttu-id="781eb-137">contact</span><span class="sxs-lookup"><span data-stu-id="781eb-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="781eb-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-138">Contacts.Read</span></span> | <span data-ttu-id="781eb-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-139">Contacts.Read</span></span> | <span data-ttu-id="781eb-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-140">Contacts.Read</span></span> |
|<span data-ttu-id="781eb-141">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="781eb-141">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="781eb-142">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-142">Not supported</span></span> | <span data-ttu-id="781eb-143">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="781eb-143">Files.ReadWrite</span></span> | <span data-ttu-id="781eb-144">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-144">Not supported</span></span> |
|<span data-ttu-id="781eb-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="781eb-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="781eb-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781eb-146">Files.ReadWrite.All</span></span> | <span data-ttu-id="781eb-147">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-147">Not supported</span></span> | <span data-ttu-id="781eb-148">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781eb-148">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="781eb-149">事件</span><span class="sxs-lookup"><span data-stu-id="781eb-149">event</span></span>](../resources/event.md) | <span data-ttu-id="781eb-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-150">Calendars.Read</span></span> | <span data-ttu-id="781eb-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-151">Calendars.Read</span></span> | <span data-ttu-id="781eb-152">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-152">Calendars.Read</span></span> |
|[<span data-ttu-id="781eb-153">组</span><span class="sxs-lookup"><span data-stu-id="781eb-153">group</span></span>](../resources/group.md) | <span data-ttu-id="781eb-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-154">Group.Read.All</span></span> | <span data-ttu-id="781eb-155">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-155">Not supported</span></span> | <span data-ttu-id="781eb-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-156">Group.Read.All</span></span> |
|[<span data-ttu-id="781eb-157">组对话</span><span class="sxs-lookup"><span data-stu-id="781eb-157">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="781eb-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-158">Group.Read.All</span></span> | <span data-ttu-id="781eb-159">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-159">Not supported</span></span> | <span data-ttu-id="781eb-160">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-160">Not supported</span></span> |
|[<span data-ttu-id="781eb-161">列表</span><span class="sxs-lookup"><span data-stu-id="781eb-161">list</span></span>](../resources/list.md) | <span data-ttu-id="781eb-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781eb-162">Sites.ReadWrite.All</span></span> | <span data-ttu-id="781eb-163">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-163">Not supported</span></span> | <span data-ttu-id="781eb-164">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781eb-164">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="781eb-165">邮件</span><span class="sxs-lookup"><span data-stu-id="781eb-165">message</span></span>](../resources/message.md) | <span data-ttu-id="781eb-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="781eb-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-167">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="781eb-168">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="781eb-168">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="781eb-169">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="781eb-169">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="781eb-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781eb-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="781eb-171">不支持</span><span class="sxs-lookup"><span data-stu-id="781eb-171">Not supported</span></span> | <span data-ttu-id="781eb-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781eb-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="781eb-173">用户</span><span class="sxs-lookup"><span data-stu-id="781eb-173">user</span></span>](../resources/user.md) | <span data-ttu-id="781eb-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-174">User.Read.All</span></span> | <span data-ttu-id="781eb-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-175">User.Read.All</span></span> | <span data-ttu-id="781eb-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="781eb-176">User.Read.All</span></span> |

> <span data-ttu-id="781eb-177">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="781eb-177">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="781eb-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="781eb-178">driveItem</span></span>

<span data-ttu-id="781eb-179">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="781eb-179">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="781eb-180">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="781eb-180">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="781eb-181">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="781eb-181">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="781eb-182">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="781eb-182">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="781eb-183">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="781eb-183">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="781eb-184">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="781eb-184">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="781eb-185">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="781eb-185">contact, event, and message</span></span>

<span data-ttu-id="781eb-186">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="781eb-186">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="781eb-187">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="781eb-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="781eb-188">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="781eb-188">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="781eb-189">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="781eb-189">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="781eb-190">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="781eb-190">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="781eb-191">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="781eb-191">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="781eb-192">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="781eb-192">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="781eb-193">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="781eb-193">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="781eb-194">请求标头</span><span class="sxs-lookup"><span data-stu-id="781eb-194">Request headers</span></span>

| <span data-ttu-id="781eb-195">名称</span><span class="sxs-lookup"><span data-stu-id="781eb-195">Name</span></span>       | <span data-ttu-id="781eb-196">类型</span><span class="sxs-lookup"><span data-stu-id="781eb-196">Type</span></span> | <span data-ttu-id="781eb-197">说明</span><span class="sxs-lookup"><span data-stu-id="781eb-197">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="781eb-198">Authorization</span><span class="sxs-lookup"><span data-stu-id="781eb-198">Authorization</span></span>  | <span data-ttu-id="781eb-199">string</span><span class="sxs-lookup"><span data-stu-id="781eb-199">string</span></span>  | <span data-ttu-id="781eb-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="781eb-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="781eb-202">响应</span><span class="sxs-lookup"><span data-stu-id="781eb-202">Response</span></span>

<span data-ttu-id="781eb-203">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="781eb-203">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="781eb-204">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="781eb-204">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="781eb-205">示例</span><span class="sxs-lookup"><span data-stu-id="781eb-205">Example</span></span>

##### <a name="request"></a><span data-ttu-id="781eb-206">请求</span><span class="sxs-lookup"><span data-stu-id="781eb-206">Request</span></span>

<span data-ttu-id="781eb-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="781eb-207">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="781eb-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="781eb-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="781eb-209">C#</span><span class="sxs-lookup"><span data-stu-id="781eb-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="781eb-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="781eb-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="781eb-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="781eb-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="781eb-212">Java</span><span class="sxs-lookup"><span data-stu-id="781eb-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="781eb-213">响应</span><span class="sxs-lookup"><span data-stu-id="781eb-213">Response</span></span>

<span data-ttu-id="781eb-214">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="781eb-214">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

