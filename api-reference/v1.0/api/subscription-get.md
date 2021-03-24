---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: 36eff9ff9f54ad6873d0948d58b7637722d9a97f
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51031119"
---
# <a name="get-subscription"></a><span data-ttu-id="479ca-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="479ca-103">Get subscription</span></span>

<span data-ttu-id="479ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="479ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="479ca-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="479ca-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="479ca-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="479ca-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="479ca-107">权限</span><span class="sxs-lookup"><span data-stu-id="479ca-107">Permissions</span></span>

<span data-ttu-id="479ca-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="479ca-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="479ca-109">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="479ca-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="479ca-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="479ca-110">Supported resource</span></span> | <span data-ttu-id="479ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="479ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="479ca-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="479ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="479ca-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="479ca-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="479ca-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="479ca-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="479ca-115">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-115">Not supported</span></span> | <span data-ttu-id="479ca-116">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-116">Not supported</span></span> | <span data-ttu-id="479ca-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-117">CallRecords.Read.All</span></span> |
|<span data-ttu-id="479ca-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="479ca-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="479ca-119">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-119">ChannelMessage.Read.All</span></span> | <span data-ttu-id="479ca-120">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-120">Not supported</span></span> |  <span data-ttu-id="479ca-121">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="479ca-122">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="479ca-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="479ca-123">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-123">Not supported</span></span> | <span data-ttu-id="479ca-124">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-124">Not supported</span></span> | <span data-ttu-id="479ca-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="479ca-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="479ca-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="479ca-127">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-127">Not supported</span></span> | <span data-ttu-id="479ca-128">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-128">Not supported</span></span> | <span data-ttu-id="479ca-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="479ca-130">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="479ca-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="479ca-131">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-131">Not supported</span></span> | <span data-ttu-id="479ca-132">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-132">Not supported</span></span> | <span data-ttu-id="479ca-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="479ca-134">contact</span><span class="sxs-lookup"><span data-stu-id="479ca-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="479ca-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-135">Contacts.Read</span></span> | <span data-ttu-id="479ca-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-136">Contacts.Read</span></span> | <span data-ttu-id="479ca-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-137">Contacts.Read</span></span> |
|<span data-ttu-id="479ca-138">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="479ca-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="479ca-139">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-139">Not supported</span></span> | <span data-ttu-id="479ca-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="479ca-140">Files.ReadWrite</span></span> | <span data-ttu-id="479ca-141">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-141">Not supported</span></span> |
|<span data-ttu-id="479ca-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="479ca-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="479ca-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="479ca-144">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-144">Not supported</span></span> | <span data-ttu-id="479ca-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="479ca-146">事件</span><span class="sxs-lookup"><span data-stu-id="479ca-146">event</span></span>](../resources/event.md) | <span data-ttu-id="479ca-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-147">Calendars.Read</span></span> | <span data-ttu-id="479ca-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-148">Calendars.Read</span></span> | <span data-ttu-id="479ca-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-149">Calendars.Read</span></span> |
|[<span data-ttu-id="479ca-150">组</span><span class="sxs-lookup"><span data-stu-id="479ca-150">group</span></span>](../resources/group.md) | <span data-ttu-id="479ca-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-151">Group.Read.All</span></span> | <span data-ttu-id="479ca-152">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-152">Not supported</span></span> | <span data-ttu-id="479ca-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-153">Group.Read.All</span></span> |
|[<span data-ttu-id="479ca-154">组对话</span><span class="sxs-lookup"><span data-stu-id="479ca-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="479ca-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-155">Group.Read.All</span></span> | <span data-ttu-id="479ca-156">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-156">Not supported</span></span> | <span data-ttu-id="479ca-157">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-157">Not supported</span></span> |
|[<span data-ttu-id="479ca-158">列表</span><span class="sxs-lookup"><span data-stu-id="479ca-158">list</span></span>](../resources/list.md) | <span data-ttu-id="479ca-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="479ca-160">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-160">Not supported</span></span> | <span data-ttu-id="479ca-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="479ca-162">邮件</span><span class="sxs-lookup"><span data-stu-id="479ca-162">message</span></span>](../resources/message.md) | <span data-ttu-id="479ca-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="479ca-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="479ca-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="479ca-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="479ca-166">打印机</span><span class="sxs-lookup"><span data-stu-id="479ca-166">printer</span></span>](../resources/printer.md) | <span data-ttu-id="479ca-167">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-167">Not supported</span></span> | <span data-ttu-id="479ca-168">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-168">Not supported</span></span> | <span data-ttu-id="479ca-169">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-169">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="479ca-170">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="479ca-170">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="479ca-171">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-171">Not supported</span></span> | <span data-ttu-id="479ca-172">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-172">Not supported</span></span> | <span data-ttu-id="479ca-173">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-173">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="479ca-174">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="479ca-174">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="479ca-175">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-175">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="479ca-176">不支持</span><span class="sxs-lookup"><span data-stu-id="479ca-176">Not supported</span></span> | <span data-ttu-id="479ca-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479ca-177">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="479ca-178">用户</span><span class="sxs-lookup"><span data-stu-id="479ca-178">user</span></span>](../resources/user.md) | <span data-ttu-id="479ca-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-179">User.Read.All</span></span> | <span data-ttu-id="479ca-180">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-180">User.Read.All</span></span> | <span data-ttu-id="479ca-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="479ca-181">User.Read.All</span></span> |

> <span data-ttu-id="479ca-182">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="479ca-182">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="479ca-183">driveItem</span><span class="sxs-lookup"><span data-stu-id="479ca-183">driveItem</span></span>

<span data-ttu-id="479ca-184">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="479ca-184">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="479ca-185">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="479ca-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="479ca-186">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="479ca-186">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="479ca-187">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="479ca-187">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="479ca-188">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="479ca-188">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="479ca-189">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="479ca-189">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="479ca-190">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="479ca-190">contact, event, and message</span></span>

<span data-ttu-id="479ca-191">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="479ca-191">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="479ca-192">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="479ca-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="479ca-193">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="479ca-193">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="479ca-194">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="479ca-194">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="479ca-195">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="479ca-195">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="479ca-196">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="479ca-196">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="479ca-197">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="479ca-197">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="479ca-198">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="479ca-198">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="479ca-199">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="479ca-199">Optional query parameters</span></span>

<span data-ttu-id="479ca-200">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="479ca-200">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="479ca-201">请求标头</span><span class="sxs-lookup"><span data-stu-id="479ca-201">Request headers</span></span>

| <span data-ttu-id="479ca-202">名称</span><span class="sxs-lookup"><span data-stu-id="479ca-202">Name</span></span>       | <span data-ttu-id="479ca-203">类型</span><span class="sxs-lookup"><span data-stu-id="479ca-203">Type</span></span> | <span data-ttu-id="479ca-204">说明</span><span class="sxs-lookup"><span data-stu-id="479ca-204">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="479ca-205">Authorization</span><span class="sxs-lookup"><span data-stu-id="479ca-205">Authorization</span></span>  | <span data-ttu-id="479ca-206">string</span><span class="sxs-lookup"><span data-stu-id="479ca-206">string</span></span>  | <span data-ttu-id="479ca-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="479ca-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="479ca-209">请求正文</span><span class="sxs-lookup"><span data-stu-id="479ca-209">Request body</span></span>

<span data-ttu-id="479ca-210">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="479ca-210">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="479ca-211">响应</span><span class="sxs-lookup"><span data-stu-id="479ca-211">Response</span></span>

<span data-ttu-id="479ca-212">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="479ca-212">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="479ca-213">示例</span><span class="sxs-lookup"><span data-stu-id="479ca-213">Example</span></span>

##### <a name="request"></a><span data-ttu-id="479ca-214">请求</span><span class="sxs-lookup"><span data-stu-id="479ca-214">Request</span></span>

<span data-ttu-id="479ca-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="479ca-215">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="479ca-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="479ca-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="479ca-217">C#</span><span class="sxs-lookup"><span data-stu-id="479ca-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="479ca-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="479ca-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="479ca-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="479ca-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="479ca-220">Java</span><span class="sxs-lookup"><span data-stu-id="479ca-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="479ca-221">响应</span><span class="sxs-lookup"><span data-stu-id="479ca-221">Response</span></span>

<span data-ttu-id="479ca-222">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="479ca-222">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false,
  "notificationContentType": "application/json"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

