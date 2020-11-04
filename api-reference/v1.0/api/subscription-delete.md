---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32a955571e0aca1eabfe899e716d658443db363b
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848196"
---
# <a name="delete-subscription"></a><span data-ttu-id="66adb-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="66adb-103">Delete subscription</span></span>

<span data-ttu-id="66adb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66adb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66adb-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="66adb-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="66adb-106">权限</span><span class="sxs-lookup"><span data-stu-id="66adb-106">Permissions</span></span>

<span data-ttu-id="66adb-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="66adb-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="66adb-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66adb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66adb-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="66adb-109">Supported resource</span></span> | <span data-ttu-id="66adb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66adb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66adb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66adb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66adb-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="66adb-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="66adb-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="66adb-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="66adb-114">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-114">Not supported</span></span> | <span data-ttu-id="66adb-115">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-115">Not supported</span></span> | <span data-ttu-id="66adb-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="66adb-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="66adb-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="66adb-118">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-118">Not supported</span></span> | <span data-ttu-id="66adb-119">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-119">Not supported</span></span> |  <span data-ttu-id="66adb-120">ChannelMessage \*、ChannelMessage \*。</span><span class="sxs-lookup"><span data-stu-id="66adb-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="66adb-121">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="66adb-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="66adb-122">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-122">Not supported</span></span> | <span data-ttu-id="66adb-123">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-123">Not supported</span></span> | <span data-ttu-id="66adb-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="66adb-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="66adb-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="66adb-126">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-126">Not supported</span></span> | <span data-ttu-id="66adb-127">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-127">Not supported</span></span> | <span data-ttu-id="66adb-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="66adb-129">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="66adb-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="66adb-130">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-130">Not supported</span></span> | <span data-ttu-id="66adb-131">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-131">Not supported</span></span> | <span data-ttu-id="66adb-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="66adb-133">contact</span><span class="sxs-lookup"><span data-stu-id="66adb-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="66adb-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-134">Contacts.Read</span></span> | <span data-ttu-id="66adb-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-135">Contacts.Read</span></span> | <span data-ttu-id="66adb-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-136">Contacts.Read</span></span> |
|<span data-ttu-id="66adb-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="66adb-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="66adb-138">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-138">Not supported</span></span> | <span data-ttu-id="66adb-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66adb-139">Files.ReadWrite</span></span> | <span data-ttu-id="66adb-140">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-140">Not supported</span></span> |
|<span data-ttu-id="66adb-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="66adb-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="66adb-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66adb-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="66adb-143">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-143">Not supported</span></span> | <span data-ttu-id="66adb-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66adb-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="66adb-145">事件</span><span class="sxs-lookup"><span data-stu-id="66adb-145">event</span></span>](../resources/event.md) | <span data-ttu-id="66adb-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-146">Calendars.Read</span></span> | <span data-ttu-id="66adb-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-147">Calendars.Read</span></span> | <span data-ttu-id="66adb-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-148">Calendars.Read</span></span> |
|[<span data-ttu-id="66adb-149">组</span><span class="sxs-lookup"><span data-stu-id="66adb-149">group</span></span>](../resources/group.md) | <span data-ttu-id="66adb-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-150">Group.Read.All</span></span> | <span data-ttu-id="66adb-151">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-151">Not supported</span></span> | <span data-ttu-id="66adb-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-152">Group.Read.All</span></span> |
|[<span data-ttu-id="66adb-153">组对话</span><span class="sxs-lookup"><span data-stu-id="66adb-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="66adb-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-154">Group.Read.All</span></span> | <span data-ttu-id="66adb-155">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-155">Not supported</span></span> | <span data-ttu-id="66adb-156">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-156">Not supported</span></span> |
|[<span data-ttu-id="66adb-157">列表</span><span class="sxs-lookup"><span data-stu-id="66adb-157">list</span></span>](../resources/list.md) | <span data-ttu-id="66adb-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66adb-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="66adb-159">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-159">Not supported</span></span> | <span data-ttu-id="66adb-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66adb-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="66adb-161">邮件</span><span class="sxs-lookup"><span data-stu-id="66adb-161">message</span></span>](../resources/message.md) | <span data-ttu-id="66adb-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="66adb-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="66adb-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66adb-164">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="66adb-165">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="66adb-165">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="66adb-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66adb-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="66adb-167">不支持</span><span class="sxs-lookup"><span data-stu-id="66adb-167">Not supported</span></span> | <span data-ttu-id="66adb-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66adb-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="66adb-169">用户</span><span class="sxs-lookup"><span data-stu-id="66adb-169">user</span></span>](../resources/user.md) | <span data-ttu-id="66adb-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-170">User.Read.All</span></span> | <span data-ttu-id="66adb-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-171">User.Read.All</span></span> | <span data-ttu-id="66adb-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="66adb-172">User.Read.All</span></span> |

> <span data-ttu-id="66adb-173">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="66adb-173">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="66adb-174">chatMessage</span><span class="sxs-lookup"><span data-stu-id="66adb-174">chatMessage</span></span>

<span data-ttu-id="66adb-175">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="66adb-175">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="66adb-176">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="66adb-176">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="66adb-177">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="66adb-177">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="66adb-178">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="66adb-178">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="66adb-179">**注意：** `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="66adb-179">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="66adb-180">driveItem</span><span class="sxs-lookup"><span data-stu-id="66adb-180">driveItem</span></span>

<span data-ttu-id="66adb-181">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="66adb-181">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="66adb-182">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="66adb-182">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="66adb-183">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="66adb-183">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="66adb-184">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="66adb-184">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="66adb-185">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="66adb-185">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="66adb-186">无法订阅不是文件夹的“ **驱动器** ”或“ **driveItem** ”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="66adb-186">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="66adb-187">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="66adb-187">contact, event, and message</span></span>

<span data-ttu-id="66adb-188">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="66adb-188">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="66adb-189">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="66adb-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="66adb-190">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="66adb-190">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="66adb-191">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="66adb-191">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="66adb-192">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="66adb-192">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="66adb-193">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="66adb-193">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="66adb-194">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="66adb-194">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="66adb-195">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66adb-195">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="66adb-196">请求标头</span><span class="sxs-lookup"><span data-stu-id="66adb-196">Request headers</span></span>

| <span data-ttu-id="66adb-197">名称</span><span class="sxs-lookup"><span data-stu-id="66adb-197">Name</span></span>       | <span data-ttu-id="66adb-198">类型</span><span class="sxs-lookup"><span data-stu-id="66adb-198">Type</span></span> | <span data-ttu-id="66adb-199">说明</span><span class="sxs-lookup"><span data-stu-id="66adb-199">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66adb-200">Authorization</span><span class="sxs-lookup"><span data-stu-id="66adb-200">Authorization</span></span>  | <span data-ttu-id="66adb-201">string</span><span class="sxs-lookup"><span data-stu-id="66adb-201">string</span></span>  | <span data-ttu-id="66adb-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66adb-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66adb-204">请求正文</span><span class="sxs-lookup"><span data-stu-id="66adb-204">Request body</span></span>

<span data-ttu-id="66adb-205">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66adb-205">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66adb-206">响应</span><span class="sxs-lookup"><span data-stu-id="66adb-206">Response</span></span>

<span data-ttu-id="66adb-207">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="66adb-207">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="66adb-208">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="66adb-208">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="66adb-209">示例</span><span class="sxs-lookup"><span data-stu-id="66adb-209">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66adb-210">请求</span><span class="sxs-lookup"><span data-stu-id="66adb-210">Request</span></span>

<span data-ttu-id="66adb-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66adb-211">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66adb-212">HTTP</span><span class="sxs-lookup"><span data-stu-id="66adb-212">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="66adb-213">C#</span><span class="sxs-lookup"><span data-stu-id="66adb-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66adb-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66adb-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66adb-215">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66adb-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66adb-216">Java</span><span class="sxs-lookup"><span data-stu-id="66adb-216">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="66adb-217">响应</span><span class="sxs-lookup"><span data-stu-id="66adb-217">Response</span></span>

<span data-ttu-id="66adb-218">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66adb-218">Here is an example of the response.</span></span>
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

