---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 08bb1904d446355dd4d953d09dc136d5b8a6008f
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394455"
---
# <a name="update-subscription"></a><span data-ttu-id="d2f64-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="d2f64-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2f64-104">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="d2f64-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="d2f64-105">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="d2f64-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="d2f64-106">为了避免丢失通知，应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="d2f64-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="d2f64-107">有关每种资源类型的最大订阅长度，请参阅[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="d2f64-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f64-108">权限</span><span class="sxs-lookup"><span data-stu-id="d2f64-108">Permissions</span></span>

<span data-ttu-id="d2f64-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="d2f64-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d2f64-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2f64-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2f64-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="d2f64-111">Supported resource</span></span> | <span data-ttu-id="d2f64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2f64-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2f64-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2f64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2f64-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2f64-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="d2f64-115">callRecord</span><span class="sxs-lookup"><span data-stu-id="d2f64-115">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="d2f64-116">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-116">Not supported</span></span> | <span data-ttu-id="d2f64-117">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-117">Not supported</span></span> | <span data-ttu-id="d2f64-118">CallRecords</span><span class="sxs-lookup"><span data-stu-id="d2f64-118">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="d2f64-119">联系人</span><span class="sxs-lookup"><span data-stu-id="d2f64-119">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d2f64-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-120">Contacts.Read</span></span> | <span data-ttu-id="d2f64-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-121">Contacts.Read</span></span> | <span data-ttu-id="d2f64-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-122">Contacts.Read</span></span> |
|<span data-ttu-id="d2f64-123">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="d2f64-123">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d2f64-124">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-124">Not supported</span></span> | <span data-ttu-id="d2f64-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2f64-125">Files.ReadWrite</span></span> | <span data-ttu-id="d2f64-126">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-126">Not supported</span></span> |
|<span data-ttu-id="d2f64-127">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="d2f64-127">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d2f64-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-128">Files.ReadWrite.All</span></span> | <span data-ttu-id="d2f64-129">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-129">Not supported</span></span> | <span data-ttu-id="d2f64-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-130">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d2f64-131">事件</span><span class="sxs-lookup"><span data-stu-id="d2f64-131">event</span></span>](../resources/event.md) | <span data-ttu-id="d2f64-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-132">Calendars.Read</span></span> | <span data-ttu-id="d2f64-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-133">Calendars.Read</span></span> | <span data-ttu-id="d2f64-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-134">Calendars.Read</span></span> |
|[<span data-ttu-id="d2f64-135">组</span><span class="sxs-lookup"><span data-stu-id="d2f64-135">group</span></span>](../resources/group.md) | <span data-ttu-id="d2f64-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-136">Group.Read.All</span></span> | <span data-ttu-id="d2f64-137">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-137">Not supported</span></span> | <span data-ttu-id="d2f64-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-138">Group.Read.All</span></span> |
|[<span data-ttu-id="d2f64-139">组对话</span><span class="sxs-lookup"><span data-stu-id="d2f64-139">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d2f64-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-140">Group.Read.All</span></span> | <span data-ttu-id="d2f64-141">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-141">Not supported</span></span> | <span data-ttu-id="d2f64-142">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-142">Not supported</span></span> |
|[<span data-ttu-id="d2f64-143">list</span><span class="sxs-lookup"><span data-stu-id="d2f64-143">list</span></span>](../resources/list.md) | <span data-ttu-id="d2f64-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-144">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d2f64-145">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-145">Not supported</span></span> | <span data-ttu-id="d2f64-146">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-146">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d2f64-147">邮件</span><span class="sxs-lookup"><span data-stu-id="d2f64-147">message</span></span>](../resources/message.md) | <span data-ttu-id="d2f64-148">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d2f64-149">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d2f64-150">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d2f64-150">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="d2f64-151">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="d2f64-151">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="d2f64-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-152">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d2f64-153">不支持</span><span class="sxs-lookup"><span data-stu-id="d2f64-153">Not supported</span></span> | <span data-ttu-id="d2f64-154">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-154">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="d2f64-155">用户</span><span class="sxs-lookup"><span data-stu-id="d2f64-155">user</span></span>](../resources/user.md) | <span data-ttu-id="d2f64-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-156">User.Read.All</span></span> | <span data-ttu-id="d2f64-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-157">User.Read.All</span></span> | <span data-ttu-id="d2f64-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f64-158">User.Read.All</span></span> |

> <span data-ttu-id="d2f64-159">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="d2f64-159">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="d2f64-160">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="d2f64-160">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="d2f64-161">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="d2f64-161">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d2f64-162">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="d2f64-162">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d2f64-163">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="d2f64-163">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="d2f64-164">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="d2f64-164">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="d2f64-165">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="d2f64-165">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d2f64-166">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="d2f64-166">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="d2f64-167">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="d2f64-167">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d2f64-168">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="d2f64-168">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d2f64-169">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="d2f64-169">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="d2f64-170">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2f64-170">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2f64-171">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2f64-171">Request headers</span></span>

| <span data-ttu-id="d2f64-172">名称</span><span class="sxs-lookup"><span data-stu-id="d2f64-172">Name</span></span>       | <span data-ttu-id="d2f64-173">类型</span><span class="sxs-lookup"><span data-stu-id="d2f64-173">Type</span></span> | <span data-ttu-id="d2f64-174">说明</span><span class="sxs-lookup"><span data-stu-id="d2f64-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2f64-175">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2f64-175">Authorization</span></span>  | <span data-ttu-id="d2f64-176">string</span><span class="sxs-lookup"><span data-stu-id="d2f64-176">string</span></span>  | <span data-ttu-id="d2f64-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2f64-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d2f64-179">响应</span><span class="sxs-lookup"><span data-stu-id="d2f64-179">Response</span></span>

<span data-ttu-id="d2f64-180">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2f64-180">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f64-181">示例</span><span class="sxs-lookup"><span data-stu-id="d2f64-181">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d2f64-182">请求</span><span class="sxs-lookup"><span data-stu-id="d2f64-182">Request</span></span>

<span data-ttu-id="d2f64-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2f64-183">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2f64-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2f64-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="d2f64-185">C#</span><span class="sxs-lookup"><span data-stu-id="d2f64-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2f64-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2f64-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2f64-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2f64-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2f64-188">响应</span><span class="sxs-lookup"><span data-stu-id="d2f64-188">Response</span></span>

<span data-ttu-id="d2f64-189">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d2f64-189">Here is an example of the response.</span></span>
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
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
