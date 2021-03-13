---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 93b614c8ba93b5643b5f630294e40fee1edf002c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761533"
---
# <a name="get-subscription"></a><span data-ttu-id="5ee7f-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="5ee7f-103">Get subscription</span></span>

<span data-ttu-id="5ee7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee7f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ee7f-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="5ee7f-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee7f-107">权限</span><span class="sxs-lookup"><span data-stu-id="5ee7f-107">Permissions</span></span>

<span data-ttu-id="5ee7f-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5ee7f-109">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ee7f-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="5ee7f-110">Supported resource</span></span> | <span data-ttu-id="5ee7f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ee7f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ee7f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ee7f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee7f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ee7f-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="5ee7f-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="5ee7f-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="5ee7f-115">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-115">Not supported</span></span> | <span data-ttu-id="5ee7f-116">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-116">Not supported</span></span> | <span data-ttu-id="5ee7f-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-117">CallRecords.Read.All</span></span> |
|<span data-ttu-id="5ee7f-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5ee7f-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="5ee7f-119">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-119">ChannelMessage.Read.All</span></span> | <span data-ttu-id="5ee7f-120">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-120">Not supported</span></span> |  <span data-ttu-id="5ee7f-121">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5ee7f-122">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="5ee7f-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="5ee7f-123">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-123">Not supported</span></span> | <span data-ttu-id="5ee7f-124">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-124">Not supported</span></span> | <span data-ttu-id="5ee7f-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5ee7f-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5ee7f-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="5ee7f-127">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-127">Not supported</span></span> | <span data-ttu-id="5ee7f-128">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-128">Not supported</span></span> | <span data-ttu-id="5ee7f-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="5ee7f-130">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="5ee7f-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="5ee7f-131">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-131">Not supported</span></span> | <span data-ttu-id="5ee7f-132">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-132">Not supported</span></span> | <span data-ttu-id="5ee7f-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="5ee7f-134">contact</span><span class="sxs-lookup"><span data-stu-id="5ee7f-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5ee7f-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-135">Contacts.Read</span></span> | <span data-ttu-id="5ee7f-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-136">Contacts.Read</span></span> | <span data-ttu-id="5ee7f-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-137">Contacts.Read</span></span> |
|<span data-ttu-id="5ee7f-138">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="5ee7f-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="5ee7f-139">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-139">Not supported</span></span> | <span data-ttu-id="5ee7f-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ee7f-140">Files.ReadWrite</span></span> | <span data-ttu-id="5ee7f-141">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-141">Not supported</span></span> |
|<span data-ttu-id="5ee7f-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="5ee7f-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="5ee7f-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="5ee7f-144">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-144">Not supported</span></span> | <span data-ttu-id="5ee7f-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="5ee7f-146">事件</span><span class="sxs-lookup"><span data-stu-id="5ee7f-146">event</span></span>](../resources/event.md) | <span data-ttu-id="5ee7f-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-147">Calendars.Read</span></span> | <span data-ttu-id="5ee7f-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-148">Calendars.Read</span></span> | <span data-ttu-id="5ee7f-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-149">Calendars.Read</span></span> |
|[<span data-ttu-id="5ee7f-150">组</span><span class="sxs-lookup"><span data-stu-id="5ee7f-150">group</span></span>](../resources/group.md) | <span data-ttu-id="5ee7f-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-151">Group.Read.All</span></span> | <span data-ttu-id="5ee7f-152">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-152">Not supported</span></span> | <span data-ttu-id="5ee7f-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-153">Group.Read.All</span></span> |
|[<span data-ttu-id="5ee7f-154">组对话</span><span class="sxs-lookup"><span data-stu-id="5ee7f-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="5ee7f-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-155">Group.Read.All</span></span> | <span data-ttu-id="5ee7f-156">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-156">Not supported</span></span> | <span data-ttu-id="5ee7f-157">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-157">Not supported</span></span> |
|[<span data-ttu-id="5ee7f-158">列表</span><span class="sxs-lookup"><span data-stu-id="5ee7f-158">list</span></span>](../resources/list.md) | <span data-ttu-id="5ee7f-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="5ee7f-160">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-160">Not supported</span></span> | <span data-ttu-id="5ee7f-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="5ee7f-162">邮件</span><span class="sxs-lookup"><span data-stu-id="5ee7f-162">message</span></span>](../resources/message.md) | <span data-ttu-id="5ee7f-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5ee7f-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5ee7f-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5ee7f-165">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="5ee7f-166">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="5ee7f-166">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="5ee7f-167">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-167">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="5ee7f-168">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee7f-168">Not supported</span></span> | <span data-ttu-id="5ee7f-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-169">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="5ee7f-170">用户</span><span class="sxs-lookup"><span data-stu-id="5ee7f-170">user</span></span>](../resources/user.md) | <span data-ttu-id="5ee7f-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-171">User.Read.All</span></span> | <span data-ttu-id="5ee7f-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-172">User.Read.All</span></span> | <span data-ttu-id="5ee7f-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee7f-173">User.Read.All</span></span> |

> <span data-ttu-id="5ee7f-174">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-174">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="5ee7f-175">driveItem</span><span class="sxs-lookup"><span data-stu-id="5ee7f-175">driveItem</span></span>

<span data-ttu-id="5ee7f-176">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-176">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="5ee7f-177">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-177">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="5ee7f-178">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-178">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="5ee7f-179">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-179">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="5ee7f-180">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-180">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="5ee7f-181">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-181">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="5ee7f-182">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="5ee7f-182">contact, event, and message</span></span>

<span data-ttu-id="5ee7f-183">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-183">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="5ee7f-184">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="5ee7f-185">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-185">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="5ee7f-186">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-186">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="5ee7f-187">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="5ee7f-187">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="5ee7f-188">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-188">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="5ee7f-189">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-189">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="5ee7f-190">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ee7f-190">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ee7f-191">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5ee7f-191">Optional query parameters</span></span>

<span data-ttu-id="5ee7f-192">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-192">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ee7f-193">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ee7f-193">Request headers</span></span>

| <span data-ttu-id="5ee7f-194">名称</span><span class="sxs-lookup"><span data-stu-id="5ee7f-194">Name</span></span>       | <span data-ttu-id="5ee7f-195">类型</span><span class="sxs-lookup"><span data-stu-id="5ee7f-195">Type</span></span> | <span data-ttu-id="5ee7f-196">说明</span><span class="sxs-lookup"><span data-stu-id="5ee7f-196">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5ee7f-197">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ee7f-197">Authorization</span></span>  | <span data-ttu-id="5ee7f-198">string</span><span class="sxs-lookup"><span data-stu-id="5ee7f-198">string</span></span>  | <span data-ttu-id="5ee7f-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ee7f-201">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ee7f-201">Request body</span></span>

<span data-ttu-id="5ee7f-202">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ee7f-203">响应</span><span class="sxs-lookup"><span data-stu-id="5ee7f-203">Response</span></span>

<span data-ttu-id="5ee7f-204">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-204">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee7f-205">示例</span><span class="sxs-lookup"><span data-stu-id="5ee7f-205">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ee7f-206">请求</span><span class="sxs-lookup"><span data-stu-id="5ee7f-206">Request</span></span>

<span data-ttu-id="5ee7f-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-207">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ee7f-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee7f-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="5ee7f-209">C#</span><span class="sxs-lookup"><span data-stu-id="5ee7f-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee7f-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee7f-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee7f-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee7f-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee7f-212">Java</span><span class="sxs-lookup"><span data-stu-id="5ee7f-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ee7f-213">响应</span><span class="sxs-lookup"><span data-stu-id="5ee7f-213">Response</span></span>

<span data-ttu-id="5ee7f-214">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-214">Here is an example of the response.</span></span>
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
  "includeResourceData": false
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

