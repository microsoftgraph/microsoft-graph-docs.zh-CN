---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 5221f855df88103808f561d720f49c812911355e
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849093"
---
# <a name="update-subscription"></a><span data-ttu-id="d55af-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="d55af-103">Update subscription</span></span>

<span data-ttu-id="d55af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d55af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d55af-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="d55af-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="d55af-106">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="d55af-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="d55af-107">为了避免丢失更改通知，应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="d55af-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="d55af-108">有关每种资源类型的最大订阅长度，请参阅 [订阅](../resources/subscription.md) 。</span><span class="sxs-lookup"><span data-stu-id="d55af-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="d55af-109">权限</span><span class="sxs-lookup"><span data-stu-id="d55af-109">Permissions</span></span>

<span data-ttu-id="d55af-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="d55af-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d55af-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d55af-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d55af-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="d55af-112">Supported resource</span></span> | <span data-ttu-id="d55af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d55af-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d55af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d55af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d55af-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d55af-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="d55af-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="d55af-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="d55af-117">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-117">Not supported</span></span> | <span data-ttu-id="d55af-118">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-118">Not supported</span></span> | <span data-ttu-id="d55af-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="d55af-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d55af-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="d55af-121">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-121">Not supported</span></span> | <span data-ttu-id="d55af-122">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-122">Not supported</span></span> |  <span data-ttu-id="d55af-123">ChannelMessage \*、ChannelMessage \*。</span><span class="sxs-lookup"><span data-stu-id="d55af-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d55af-124">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="d55af-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="d55af-125">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-125">Not supported</span></span> | <span data-ttu-id="d55af-126">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-126">Not supported</span></span> | <span data-ttu-id="d55af-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d55af-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d55af-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="d55af-129">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-129">Not supported</span></span> | <span data-ttu-id="d55af-130">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-130">Not supported</span></span> | <span data-ttu-id="d55af-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="d55af-132">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="d55af-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="d55af-133">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-133">Not supported</span></span> | <span data-ttu-id="d55af-134">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-134">Not supported</span></span> | <span data-ttu-id="d55af-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="d55af-136">contact</span><span class="sxs-lookup"><span data-stu-id="d55af-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d55af-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-137">Contacts.Read</span></span> | <span data-ttu-id="d55af-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-138">Contacts.Read</span></span> | <span data-ttu-id="d55af-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-139">Contacts.Read</span></span> |
|<span data-ttu-id="d55af-140">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="d55af-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d55af-141">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-141">Not supported</span></span> | <span data-ttu-id="d55af-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d55af-142">Files.ReadWrite</span></span> | <span data-ttu-id="d55af-143">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-143">Not supported</span></span> |
|<span data-ttu-id="d55af-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="d55af-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d55af-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55af-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="d55af-146">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-146">Not supported</span></span> | <span data-ttu-id="d55af-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55af-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d55af-148">事件</span><span class="sxs-lookup"><span data-stu-id="d55af-148">event</span></span>](../resources/event.md) | <span data-ttu-id="d55af-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-149">Calendars.Read</span></span> | <span data-ttu-id="d55af-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-150">Calendars.Read</span></span> | <span data-ttu-id="d55af-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-151">Calendars.Read</span></span> |
|[<span data-ttu-id="d55af-152">组</span><span class="sxs-lookup"><span data-stu-id="d55af-152">group</span></span>](../resources/group.md) | <span data-ttu-id="d55af-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-153">Group.Read.All</span></span> | <span data-ttu-id="d55af-154">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-154">Not supported</span></span> | <span data-ttu-id="d55af-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-155">Group.Read.All</span></span> |
|[<span data-ttu-id="d55af-156">组对话</span><span class="sxs-lookup"><span data-stu-id="d55af-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d55af-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-157">Group.Read.All</span></span> | <span data-ttu-id="d55af-158">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-158">Not supported</span></span> | <span data-ttu-id="d55af-159">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-159">Not supported</span></span> |
|[<span data-ttu-id="d55af-160">列表</span><span class="sxs-lookup"><span data-stu-id="d55af-160">list</span></span>](../resources/list.md) | <span data-ttu-id="d55af-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55af-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d55af-162">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-162">Not supported</span></span> | <span data-ttu-id="d55af-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55af-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d55af-164">邮件</span><span class="sxs-lookup"><span data-stu-id="d55af-164">message</span></span>](../resources/message.md) | <span data-ttu-id="d55af-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d55af-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d55af-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d55af-167">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="d55af-168">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="d55af-168">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="d55af-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55af-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d55af-170">不支持</span><span class="sxs-lookup"><span data-stu-id="d55af-170">Not supported</span></span> | <span data-ttu-id="d55af-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55af-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="d55af-172">用户</span><span class="sxs-lookup"><span data-stu-id="d55af-172">user</span></span>](../resources/user.md) | <span data-ttu-id="d55af-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-173">User.Read.All</span></span> | <span data-ttu-id="d55af-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-174">User.Read.All</span></span> | <span data-ttu-id="d55af-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55af-175">User.Read.All</span></span> |

> <span data-ttu-id="d55af-176">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="d55af-176">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="d55af-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d55af-177">chatMessage</span></span>

<span data-ttu-id="d55af-178">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="d55af-178">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="d55af-179">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="d55af-179">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="d55af-180">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="d55af-180">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="d55af-181">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="d55af-181">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="d55af-182">**注意：** `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="d55af-182">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="d55af-183">driveItem</span><span class="sxs-lookup"><span data-stu-id="d55af-183">driveItem</span></span>

<span data-ttu-id="d55af-184">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="d55af-184">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="d55af-185">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="d55af-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="d55af-186">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="d55af-186">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d55af-187">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="d55af-187">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d55af-188">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="d55af-188">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="d55af-189">无法订阅不是文件夹的“ **驱动器** ”或“ **driveItem** ”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="d55af-189">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="d55af-190">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="d55af-190">contact, event, and message</span></span>

<span data-ttu-id="d55af-191">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="d55af-191">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="d55af-192">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="d55af-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="d55af-193">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="d55af-193">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d55af-194">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="d55af-194">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="d55af-195">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="d55af-195">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d55af-196">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="d55af-196">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d55af-197">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="d55af-197">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="d55af-198">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d55af-198">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d55af-199">请求标头</span><span class="sxs-lookup"><span data-stu-id="d55af-199">Request headers</span></span>

| <span data-ttu-id="d55af-200">名称</span><span class="sxs-lookup"><span data-stu-id="d55af-200">Name</span></span>       | <span data-ttu-id="d55af-201">类型</span><span class="sxs-lookup"><span data-stu-id="d55af-201">Type</span></span> | <span data-ttu-id="d55af-202">说明</span><span class="sxs-lookup"><span data-stu-id="d55af-202">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d55af-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="d55af-203">Authorization</span></span>  | <span data-ttu-id="d55af-204">string</span><span class="sxs-lookup"><span data-stu-id="d55af-204">string</span></span>  | <span data-ttu-id="d55af-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d55af-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d55af-207">响应</span><span class="sxs-lookup"><span data-stu-id="d55af-207">Response</span></span>

<span data-ttu-id="d55af-208">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d55af-208">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="d55af-209">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="d55af-209">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="d55af-210">示例</span><span class="sxs-lookup"><span data-stu-id="d55af-210">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d55af-211">请求</span><span class="sxs-lookup"><span data-stu-id="d55af-211">Request</span></span>

<span data-ttu-id="d55af-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d55af-212">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d55af-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="d55af-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d55af-214">C#</span><span class="sxs-lookup"><span data-stu-id="d55af-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d55af-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d55af-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d55af-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d55af-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d55af-217">Java</span><span class="sxs-lookup"><span data-stu-id="d55af-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d55af-218">响应</span><span class="sxs-lookup"><span data-stu-id="d55af-218">Response</span></span>

<span data-ttu-id="d55af-219">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d55af-219">Here is an example of the response.</span></span>
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

