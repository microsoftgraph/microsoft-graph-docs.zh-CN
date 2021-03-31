---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: Jumaodhiss
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: 3b00e7d72833e1f871b59aa0a906a295d42fbc5f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468819"
---
# <a name="update-subscription"></a><span data-ttu-id="a5804-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="a5804-103">Update subscription</span></span>

<span data-ttu-id="a5804-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5804-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5804-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="a5804-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="a5804-106">"权限 ["部分](#permissions) 中的表列出了支持订阅更改通知的资源。</span><span class="sxs-lookup"><span data-stu-id="a5804-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="a5804-107">订阅在时间长度因资源类型而异后过期。</span><span class="sxs-lookup"><span data-stu-id="a5804-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="a5804-108">为了避免缺少更改通知，应用应在到期日期之前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="a5804-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="a5804-109">请参阅 [订阅](../resources/subscription.md) ，了解每种资源类型的订阅的最大长度。</span><span class="sxs-lookup"><span data-stu-id="a5804-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5804-110">权限</span><span class="sxs-lookup"><span data-stu-id="a5804-110">Permissions</span></span>

<span data-ttu-id="a5804-111">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="a5804-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a5804-112">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5804-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5804-113">支持的资源</span><span class="sxs-lookup"><span data-stu-id="a5804-113">Supported resource</span></span> | <span data-ttu-id="a5804-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5804-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a5804-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5804-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5804-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5804-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="a5804-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="a5804-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="a5804-118">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-118">Not supported</span></span> | <span data-ttu-id="a5804-119">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-119">Not supported</span></span> | <span data-ttu-id="a5804-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="a5804-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a5804-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="a5804-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-122">ChannelMessage.Read.All</span></span> | <span data-ttu-id="a5804-123">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-123">Not supported</span></span> |  <span data-ttu-id="a5804-124">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a5804-125">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="a5804-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="a5804-126">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-126">Not supported</span></span> | <span data-ttu-id="a5804-127">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-127">Not supported</span></span> | <span data-ttu-id="a5804-128">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-128">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a5804-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a5804-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="a5804-130">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-130">Not supported</span></span> | <span data-ttu-id="a5804-131">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-131">Not supported</span></span> | <span data-ttu-id="a5804-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-132">Chat.Read.All</span></span>  |
|<span data-ttu-id="a5804-133">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="a5804-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="a5804-134">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-134">Not supported</span></span> | <span data-ttu-id="a5804-135">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-135">Not supported</span></span> | <span data-ttu-id="a5804-136">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-136">Chat.Read.All</span></span>  |
|[<span data-ttu-id="a5804-137">contact</span><span class="sxs-lookup"><span data-stu-id="a5804-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a5804-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-138">Contacts.Read</span></span> | <span data-ttu-id="a5804-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-139">Contacts.Read</span></span> | <span data-ttu-id="a5804-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-140">Contacts.Read</span></span> |
|<span data-ttu-id="a5804-141">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="a5804-141">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a5804-142">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-142">Not supported</span></span> | <span data-ttu-id="a5804-143">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5804-143">Files.ReadWrite</span></span> | <span data-ttu-id="a5804-144">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-144">Not supported</span></span> |
|<span data-ttu-id="a5804-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="a5804-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a5804-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-146">Files.ReadWrite.All</span></span> | <span data-ttu-id="a5804-147">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-147">Not supported</span></span> | <span data-ttu-id="a5804-148">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-148">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a5804-149">事件</span><span class="sxs-lookup"><span data-stu-id="a5804-149">event</span></span>](../resources/event.md) | <span data-ttu-id="a5804-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-150">Calendars.Read</span></span> | <span data-ttu-id="a5804-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-151">Calendars.Read</span></span> | <span data-ttu-id="a5804-152">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-152">Calendars.Read</span></span> |
|[<span data-ttu-id="a5804-153">组</span><span class="sxs-lookup"><span data-stu-id="a5804-153">group</span></span>](../resources/group.md) | <span data-ttu-id="a5804-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-154">Group.Read.All</span></span> | <span data-ttu-id="a5804-155">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-155">Not supported</span></span> | <span data-ttu-id="a5804-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-156">Group.Read.All</span></span> |
|[<span data-ttu-id="a5804-157">组对话</span><span class="sxs-lookup"><span data-stu-id="a5804-157">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a5804-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-158">Group.Read.All</span></span> | <span data-ttu-id="a5804-159">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-159">Not supported</span></span> | <span data-ttu-id="a5804-160">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-160">Not supported</span></span> |
|[<span data-ttu-id="a5804-161">列表</span><span class="sxs-lookup"><span data-stu-id="a5804-161">list</span></span>](../resources/list.md) | <span data-ttu-id="a5804-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-162">Sites.ReadWrite.All</span></span> | <span data-ttu-id="a5804-163">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-163">Not supported</span></span> | <span data-ttu-id="a5804-164">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-164">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="a5804-165">邮件</span><span class="sxs-lookup"><span data-stu-id="a5804-165">message</span></span>](../resources/message.md) | <span data-ttu-id="a5804-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a5804-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-167">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a5804-168">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a5804-168">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="a5804-169">打印机</span><span class="sxs-lookup"><span data-stu-id="a5804-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="a5804-170">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-170">Not supported</span></span> | <span data-ttu-id="a5804-171">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-171">Not supported</span></span> | <span data-ttu-id="a5804-172">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="a5804-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="a5804-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="a5804-174">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-174">Not supported</span></span> | <span data-ttu-id="a5804-175">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-175">Not supported</span></span> | <span data-ttu-id="a5804-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="a5804-177">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="a5804-177">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="a5804-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a5804-179">不支持</span><span class="sxs-lookup"><span data-stu-id="a5804-179">Not supported</span></span> | <span data-ttu-id="a5804-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5804-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a5804-181">用户</span><span class="sxs-lookup"><span data-stu-id="a5804-181">user</span></span>](../resources/user.md) | <span data-ttu-id="a5804-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-182">User.Read.All</span></span> | <span data-ttu-id="a5804-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-183">User.Read.All</span></span> | <span data-ttu-id="a5804-184">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5804-184">User.Read.All</span></span> |

> <span data-ttu-id="a5804-185">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="a5804-185">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="a5804-186">driveItem</span><span class="sxs-lookup"><span data-stu-id="a5804-186">driveItem</span></span>

<span data-ttu-id="a5804-187">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="a5804-187">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="a5804-188">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="a5804-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="a5804-189">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="a5804-189">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a5804-190">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="a5804-190">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a5804-191">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="a5804-191">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="a5804-192">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="a5804-192">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="a5804-193">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="a5804-193">contact, event, and message</span></span>

<span data-ttu-id="a5804-194">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="a5804-194">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="a5804-195">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="a5804-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="a5804-196">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="a5804-196">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a5804-197">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="a5804-197">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a5804-198">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="a5804-198">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a5804-199">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="a5804-199">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a5804-200">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="a5804-200">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="a5804-201">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5804-201">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5804-202">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5804-202">Request headers</span></span>

| <span data-ttu-id="a5804-203">名称</span><span class="sxs-lookup"><span data-stu-id="a5804-203">Name</span></span>       | <span data-ttu-id="a5804-204">类型</span><span class="sxs-lookup"><span data-stu-id="a5804-204">Type</span></span> | <span data-ttu-id="a5804-205">说明</span><span class="sxs-lookup"><span data-stu-id="a5804-205">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5804-206">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5804-206">Authorization</span></span>  | <span data-ttu-id="a5804-207">string</span><span class="sxs-lookup"><span data-stu-id="a5804-207">string</span></span>  | <span data-ttu-id="a5804-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5804-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a5804-210">响应</span><span class="sxs-lookup"><span data-stu-id="a5804-210">Response</span></span>

<span data-ttu-id="a5804-211">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a5804-211">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="a5804-212">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="a5804-212">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="a5804-213">示例</span><span class="sxs-lookup"><span data-stu-id="a5804-213">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5804-214">请求</span><span class="sxs-lookup"><span data-stu-id="a5804-214">Request</span></span>

<span data-ttu-id="a5804-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5804-215">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5804-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5804-216">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a5804-217">C#</span><span class="sxs-lookup"><span data-stu-id="a5804-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5804-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5804-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5804-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5804-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5804-220">Java</span><span class="sxs-lookup"><span data-stu-id="a5804-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5804-221">响应</span><span class="sxs-lookup"><span data-stu-id="a5804-221">Response</span></span>

<span data-ttu-id="a5804-222">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a5804-222">Here is an example of the response.</span></span>
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
  "includeResourceData": false,
  "notificationContentType": "application/json"
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

