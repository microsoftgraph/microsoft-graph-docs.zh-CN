---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4550912f9f4392131e62cb26a3328698bf121c15
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034280"
---
# <a name="get-subscription"></a><span data-ttu-id="584e2-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="584e2-103">Get subscription</span></span>

<span data-ttu-id="584e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="584e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="584e2-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="584e2-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="584e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="584e2-106">Permissions</span></span>

<span data-ttu-id="584e2-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="584e2-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="584e2-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="584e2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="584e2-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="584e2-109">Supported resource</span></span> | <span data-ttu-id="584e2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="584e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="584e2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="584e2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="584e2-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="584e2-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="584e2-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="584e2-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="584e2-114">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-114">Not supported</span></span> | <span data-ttu-id="584e2-115">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-115">Not supported</span></span> | <span data-ttu-id="584e2-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="584e2-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="584e2-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="584e2-118">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-118">Not supported</span></span> | <span data-ttu-id="584e2-119">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-119">Not supported</span></span> |  <span data-ttu-id="584e2-120">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="584e2-121">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="584e2-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="584e2-122">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-122">Not supported</span></span> | <span data-ttu-id="584e2-123">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-123">Not supported</span></span> | <span data-ttu-id="584e2-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="584e2-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="584e2-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="584e2-126">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-126">Not supported</span></span> | <span data-ttu-id="584e2-127">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-127">Not supported</span></span> | <span data-ttu-id="584e2-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="584e2-129">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="584e2-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="584e2-130">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-130">Not supported</span></span> | <span data-ttu-id="584e2-131">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-131">Not supported</span></span> | <span data-ttu-id="584e2-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="584e2-133">contact</span><span class="sxs-lookup"><span data-stu-id="584e2-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="584e2-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-134">Contacts.Read</span></span> | <span data-ttu-id="584e2-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-135">Contacts.Read</span></span> | <span data-ttu-id="584e2-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-136">Contacts.Read</span></span> |
|<span data-ttu-id="584e2-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="584e2-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="584e2-138">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-138">Not supported</span></span> | <span data-ttu-id="584e2-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="584e2-139">Files.ReadWrite</span></span> | <span data-ttu-id="584e2-140">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-140">Not supported</span></span> |
|<span data-ttu-id="584e2-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="584e2-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="584e2-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584e2-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="584e2-143">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-143">Not supported</span></span> | <span data-ttu-id="584e2-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584e2-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="584e2-145">事件</span><span class="sxs-lookup"><span data-stu-id="584e2-145">event</span></span>](../resources/event.md) | <span data-ttu-id="584e2-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-146">Calendars.Read</span></span> | <span data-ttu-id="584e2-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-147">Calendars.Read</span></span> | <span data-ttu-id="584e2-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-148">Calendars.Read</span></span> |
|[<span data-ttu-id="584e2-149">组</span><span class="sxs-lookup"><span data-stu-id="584e2-149">group</span></span>](../resources/group.md) | <span data-ttu-id="584e2-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-150">Group.Read.All</span></span> | <span data-ttu-id="584e2-151">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-151">Not supported</span></span> | <span data-ttu-id="584e2-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-152">Group.Read.All</span></span> |
|[<span data-ttu-id="584e2-153">组对话</span><span class="sxs-lookup"><span data-stu-id="584e2-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="584e2-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-154">Group.Read.All</span></span> | <span data-ttu-id="584e2-155">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-155">Not supported</span></span> | <span data-ttu-id="584e2-156">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-156">Not supported</span></span> |
|[<span data-ttu-id="584e2-157">列表</span><span class="sxs-lookup"><span data-stu-id="584e2-157">list</span></span>](../resources/list.md) | <span data-ttu-id="584e2-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584e2-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="584e2-159">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-159">Not supported</span></span> | <span data-ttu-id="584e2-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584e2-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="584e2-161">邮件</span><span class="sxs-lookup"><span data-stu-id="584e2-161">message</span></span>](../resources/message.md) | <span data-ttu-id="584e2-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="584e2-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="584e2-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="584e2-164">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="584e2-165">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="584e2-165">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="584e2-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584e2-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="584e2-167">不支持</span><span class="sxs-lookup"><span data-stu-id="584e2-167">Not supported</span></span> | <span data-ttu-id="584e2-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584e2-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="584e2-169">用户</span><span class="sxs-lookup"><span data-stu-id="584e2-169">user</span></span>](../resources/user.md) | <span data-ttu-id="584e2-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-170">User.Read.All</span></span> | <span data-ttu-id="584e2-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-171">User.Read.All</span></span> | <span data-ttu-id="584e2-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="584e2-172">User.Read.All</span></span> |

> <span data-ttu-id="584e2-173">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="584e2-173">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="584e2-174">driveItem</span><span class="sxs-lookup"><span data-stu-id="584e2-174">driveItem</span></span>

<span data-ttu-id="584e2-175">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="584e2-175">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="584e2-176">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="584e2-176">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="584e2-177">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="584e2-177">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="584e2-178">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="584e2-178">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="584e2-179">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="584e2-179">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="584e2-180">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="584e2-180">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="584e2-181">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="584e2-181">contact, event, and message</span></span>

<span data-ttu-id="584e2-182">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="584e2-182">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="584e2-183">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="584e2-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="584e2-184">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="584e2-184">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="584e2-185">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="584e2-185">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="584e2-186">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="584e2-186">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="584e2-187">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="584e2-187">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="584e2-188">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="584e2-188">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="584e2-189">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="584e2-189">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="584e2-190">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="584e2-190">Optional query parameters</span></span>

<span data-ttu-id="584e2-191">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="584e2-191">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="584e2-192">请求标头</span><span class="sxs-lookup"><span data-stu-id="584e2-192">Request headers</span></span>

| <span data-ttu-id="584e2-193">名称</span><span class="sxs-lookup"><span data-stu-id="584e2-193">Name</span></span>       | <span data-ttu-id="584e2-194">类型</span><span class="sxs-lookup"><span data-stu-id="584e2-194">Type</span></span> | <span data-ttu-id="584e2-195">说明</span><span class="sxs-lookup"><span data-stu-id="584e2-195">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="584e2-196">Authorization</span><span class="sxs-lookup"><span data-stu-id="584e2-196">Authorization</span></span>  | <span data-ttu-id="584e2-197">string</span><span class="sxs-lookup"><span data-stu-id="584e2-197">string</span></span>  | <span data-ttu-id="584e2-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="584e2-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="584e2-200">请求正文</span><span class="sxs-lookup"><span data-stu-id="584e2-200">Request body</span></span>

<span data-ttu-id="584e2-201">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="584e2-201">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="584e2-202">响应</span><span class="sxs-lookup"><span data-stu-id="584e2-202">Response</span></span>

<span data-ttu-id="584e2-203">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="584e2-203">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="584e2-204">示例</span><span class="sxs-lookup"><span data-stu-id="584e2-204">Example</span></span>

##### <a name="request"></a><span data-ttu-id="584e2-205">请求</span><span class="sxs-lookup"><span data-stu-id="584e2-205">Request</span></span>

<span data-ttu-id="584e2-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="584e2-206">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="584e2-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="584e2-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="584e2-208">C#</span><span class="sxs-lookup"><span data-stu-id="584e2-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="584e2-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="584e2-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="584e2-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="584e2-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="584e2-211">Java</span><span class="sxs-lookup"><span data-stu-id="584e2-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="584e2-212">响应</span><span class="sxs-lookup"><span data-stu-id="584e2-212">Response</span></span>

<span data-ttu-id="584e2-213">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="584e2-213">Here is an example of the response.</span></span>
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

