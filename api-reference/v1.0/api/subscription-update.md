---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c2f5e7aa89b68c911e79b5d2a9909d398d3f58b6
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034171"
---
# <a name="update-subscription"></a><span data-ttu-id="7446f-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="7446f-103">Update subscription</span></span>

<span data-ttu-id="7446f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7446f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7446f-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="7446f-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="7446f-106">订阅在时间长度因资源类型而异后过期。</span><span class="sxs-lookup"><span data-stu-id="7446f-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="7446f-107">为了避免缺少更改通知，应用应在到期日期之前很好地续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="7446f-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="7446f-108">请参阅 [订阅](../resources/subscription.md) ，了解每种资源类型的订阅的最大长度。</span><span class="sxs-lookup"><span data-stu-id="7446f-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="7446f-109">权限</span><span class="sxs-lookup"><span data-stu-id="7446f-109">Permissions</span></span>

<span data-ttu-id="7446f-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="7446f-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7446f-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7446f-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7446f-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="7446f-112">Supported resource</span></span> | <span data-ttu-id="7446f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7446f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7446f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7446f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7446f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7446f-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="7446f-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="7446f-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="7446f-117">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-117">Not supported</span></span> | <span data-ttu-id="7446f-118">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-118">Not supported</span></span> | <span data-ttu-id="7446f-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="7446f-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7446f-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="7446f-121">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-121">Not supported</span></span> | <span data-ttu-id="7446f-122">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-122">Not supported</span></span> |  <span data-ttu-id="7446f-123">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7446f-124">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="7446f-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="7446f-125">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-125">Not supported</span></span> | <span data-ttu-id="7446f-126">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-126">Not supported</span></span> | <span data-ttu-id="7446f-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7446f-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7446f-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="7446f-129">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-129">Not supported</span></span> | <span data-ttu-id="7446f-130">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-130">Not supported</span></span> | <span data-ttu-id="7446f-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="7446f-132">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="7446f-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="7446f-133">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-133">Not supported</span></span> | <span data-ttu-id="7446f-134">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-134">Not supported</span></span> | <span data-ttu-id="7446f-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="7446f-136">contact</span><span class="sxs-lookup"><span data-stu-id="7446f-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="7446f-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-137">Contacts.Read</span></span> | <span data-ttu-id="7446f-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-138">Contacts.Read</span></span> | <span data-ttu-id="7446f-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-139">Contacts.Read</span></span> |
|<span data-ttu-id="7446f-140">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="7446f-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="7446f-141">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-141">Not supported</span></span> | <span data-ttu-id="7446f-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7446f-142">Files.ReadWrite</span></span> | <span data-ttu-id="7446f-143">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-143">Not supported</span></span> |
|<span data-ttu-id="7446f-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="7446f-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="7446f-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7446f-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="7446f-146">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-146">Not supported</span></span> | <span data-ttu-id="7446f-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7446f-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="7446f-148">事件</span><span class="sxs-lookup"><span data-stu-id="7446f-148">event</span></span>](../resources/event.md) | <span data-ttu-id="7446f-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-149">Calendars.Read</span></span> | <span data-ttu-id="7446f-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-150">Calendars.Read</span></span> | <span data-ttu-id="7446f-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-151">Calendars.Read</span></span> |
|[<span data-ttu-id="7446f-152">组</span><span class="sxs-lookup"><span data-stu-id="7446f-152">group</span></span>](../resources/group.md) | <span data-ttu-id="7446f-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-153">Group.Read.All</span></span> | <span data-ttu-id="7446f-154">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-154">Not supported</span></span> | <span data-ttu-id="7446f-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-155">Group.Read.All</span></span> |
|[<span data-ttu-id="7446f-156">组对话</span><span class="sxs-lookup"><span data-stu-id="7446f-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="7446f-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-157">Group.Read.All</span></span> | <span data-ttu-id="7446f-158">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-158">Not supported</span></span> | <span data-ttu-id="7446f-159">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-159">Not supported</span></span> |
|[<span data-ttu-id="7446f-160">列表</span><span class="sxs-lookup"><span data-stu-id="7446f-160">list</span></span>](../resources/list.md) | <span data-ttu-id="7446f-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7446f-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="7446f-162">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-162">Not supported</span></span> | <span data-ttu-id="7446f-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7446f-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="7446f-164">邮件</span><span class="sxs-lookup"><span data-stu-id="7446f-164">message</span></span>](../resources/message.md) | <span data-ttu-id="7446f-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7446f-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7446f-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7446f-167">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="7446f-168">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="7446f-168">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="7446f-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7446f-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="7446f-170">不支持</span><span class="sxs-lookup"><span data-stu-id="7446f-170">Not supported</span></span> | <span data-ttu-id="7446f-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7446f-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="7446f-172">用户</span><span class="sxs-lookup"><span data-stu-id="7446f-172">user</span></span>](../resources/user.md) | <span data-ttu-id="7446f-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-173">User.Read.All</span></span> | <span data-ttu-id="7446f-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-174">User.Read.All</span></span> | <span data-ttu-id="7446f-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7446f-175">User.Read.All</span></span> |

> <span data-ttu-id="7446f-176">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="7446f-176">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="7446f-177">driveItem</span><span class="sxs-lookup"><span data-stu-id="7446f-177">driveItem</span></span>

<span data-ttu-id="7446f-178">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="7446f-178">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="7446f-179">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="7446f-179">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="7446f-180">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="7446f-180">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="7446f-181">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="7446f-181">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="7446f-182">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="7446f-182">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="7446f-183">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="7446f-183">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="7446f-184">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="7446f-184">contact, event, and message</span></span>

<span data-ttu-id="7446f-185">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="7446f-185">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="7446f-186">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="7446f-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="7446f-187">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="7446f-187">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="7446f-188">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="7446f-188">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="7446f-189">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="7446f-189">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="7446f-190">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="7446f-190">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="7446f-191">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="7446f-191">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="7446f-192">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7446f-192">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7446f-193">请求标头</span><span class="sxs-lookup"><span data-stu-id="7446f-193">Request headers</span></span>

| <span data-ttu-id="7446f-194">名称</span><span class="sxs-lookup"><span data-stu-id="7446f-194">Name</span></span>       | <span data-ttu-id="7446f-195">类型</span><span class="sxs-lookup"><span data-stu-id="7446f-195">Type</span></span> | <span data-ttu-id="7446f-196">说明</span><span class="sxs-lookup"><span data-stu-id="7446f-196">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7446f-197">Authorization</span><span class="sxs-lookup"><span data-stu-id="7446f-197">Authorization</span></span>  | <span data-ttu-id="7446f-198">string</span><span class="sxs-lookup"><span data-stu-id="7446f-198">string</span></span>  | <span data-ttu-id="7446f-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7446f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7446f-201">响应</span><span class="sxs-lookup"><span data-stu-id="7446f-201">Response</span></span>

<span data-ttu-id="7446f-202">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7446f-202">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="7446f-203">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="7446f-203">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="7446f-204">示例</span><span class="sxs-lookup"><span data-stu-id="7446f-204">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7446f-205">请求</span><span class="sxs-lookup"><span data-stu-id="7446f-205">Request</span></span>

<span data-ttu-id="7446f-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7446f-206">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7446f-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="7446f-207">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7446f-208">C#</span><span class="sxs-lookup"><span data-stu-id="7446f-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7446f-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7446f-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7446f-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7446f-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7446f-211">Java</span><span class="sxs-lookup"><span data-stu-id="7446f-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7446f-212">响应</span><span class="sxs-lookup"><span data-stu-id="7446f-212">Response</span></span>

<span data-ttu-id="7446f-213">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7446f-213">Here is an example of the response.</span></span>
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

