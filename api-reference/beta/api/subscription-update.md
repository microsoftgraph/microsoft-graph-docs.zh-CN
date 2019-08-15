---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 31636d6b40fd952cb629f2fe309eec887bc22e30
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409833"
---
# <a name="update-subscription"></a><span data-ttu-id="4800e-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="4800e-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4800e-104">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="4800e-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="4800e-105">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="4800e-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="4800e-106">为了避免丢失通知, 应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="4800e-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="4800e-107">有关每种资源类型的最大订阅长度, 请参阅[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="4800e-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="4800e-108">权限</span><span class="sxs-lookup"><span data-stu-id="4800e-108">Permissions</span></span>

<span data-ttu-id="4800e-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="4800e-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4800e-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4800e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4800e-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="4800e-111">Supported resource</span></span> | <span data-ttu-id="4800e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4800e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4800e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4800e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4800e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4800e-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="4800e-115">联系人</span><span class="sxs-lookup"><span data-stu-id="4800e-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="4800e-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-116">Contacts.Read</span></span> | <span data-ttu-id="4800e-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-117">Contacts.Read</span></span> | <span data-ttu-id="4800e-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-118">Contacts.Read</span></span> |
|<span data-ttu-id="4800e-119">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="4800e-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="4800e-120">不支持</span><span class="sxs-lookup"><span data-stu-id="4800e-120">Not supported</span></span> | <span data-ttu-id="4800e-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4800e-121">Files.ReadWrite</span></span> | <span data-ttu-id="4800e-122">不支持</span><span class="sxs-lookup"><span data-stu-id="4800e-122">Not supported</span></span> |
|<span data-ttu-id="4800e-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="4800e-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="4800e-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4800e-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="4800e-125">不支持</span><span class="sxs-lookup"><span data-stu-id="4800e-125">Not supported</span></span> | <span data-ttu-id="4800e-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4800e-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="4800e-127">事件</span><span class="sxs-lookup"><span data-stu-id="4800e-127">event</span></span>](../resources/event.md) | <span data-ttu-id="4800e-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-128">Calendars.Read</span></span> | <span data-ttu-id="4800e-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-129">Calendars.Read</span></span> | <span data-ttu-id="4800e-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-130">Calendars.Read</span></span> |
|[<span data-ttu-id="4800e-131">组</span><span class="sxs-lookup"><span data-stu-id="4800e-131">group</span></span>](../resources/group.md) | <span data-ttu-id="4800e-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4800e-132">Group.Read.All</span></span> | <span data-ttu-id="4800e-133">不支持</span><span class="sxs-lookup"><span data-stu-id="4800e-133">Not supported</span></span> | <span data-ttu-id="4800e-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4800e-134">Group.Read.All</span></span> |
|[<span data-ttu-id="4800e-135">组对话</span><span class="sxs-lookup"><span data-stu-id="4800e-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="4800e-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4800e-136">Group.Read.All</span></span> | <span data-ttu-id="4800e-137">不支持</span><span class="sxs-lookup"><span data-stu-id="4800e-137">Not supported</span></span> | <span data-ttu-id="4800e-138">不支持</span><span class="sxs-lookup"><span data-stu-id="4800e-138">Not supported</span></span> |
|[<span data-ttu-id="4800e-139">邮件</span><span class="sxs-lookup"><span data-stu-id="4800e-139">message</span></span>](../resources/message.md) | <span data-ttu-id="4800e-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-140">Mail.Read</span></span> | <span data-ttu-id="4800e-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-141">Mail.Read</span></span> | <span data-ttu-id="4800e-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4800e-142">Mail.Read</span></span> |
|<span data-ttu-id="4800e-143">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="4800e-143">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="4800e-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4800e-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="4800e-145">不支持</span><span class="sxs-lookup"><span data-stu-id="4800e-145">Not supported</span></span> | <span data-ttu-id="4800e-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4800e-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="4800e-147">用户</span><span class="sxs-lookup"><span data-stu-id="4800e-147">user</span></span>](../resources/user.md) | <span data-ttu-id="4800e-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4800e-148">User.Read.All</span></span> | <span data-ttu-id="4800e-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4800e-149">User.Read.All</span></span> | <span data-ttu-id="4800e-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4800e-150">User.Read.All</span></span> |

> <span data-ttu-id="4800e-151">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="4800e-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="4800e-152">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="4800e-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="4800e-153">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="4800e-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="4800e-154">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="4800e-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="4800e-155">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="4800e-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="4800e-156">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="4800e-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="4800e-157">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="4800e-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="4800e-158">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="4800e-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="4800e-159">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="4800e-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="4800e-160">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="4800e-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="4800e-161">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="4800e-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="4800e-162">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4800e-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4800e-163">请求标头</span><span class="sxs-lookup"><span data-stu-id="4800e-163">Request headers</span></span>

| <span data-ttu-id="4800e-164">名称</span><span class="sxs-lookup"><span data-stu-id="4800e-164">Name</span></span>       | <span data-ttu-id="4800e-165">类型</span><span class="sxs-lookup"><span data-stu-id="4800e-165">Type</span></span> | <span data-ttu-id="4800e-166">说明</span><span class="sxs-lookup"><span data-stu-id="4800e-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4800e-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="4800e-167">Authorization</span></span>  | <span data-ttu-id="4800e-168">string</span><span class="sxs-lookup"><span data-stu-id="4800e-168">string</span></span>  | <span data-ttu-id="4800e-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4800e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4800e-171">响应</span><span class="sxs-lookup"><span data-stu-id="4800e-171">Response</span></span>

<span data-ttu-id="4800e-172">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4800e-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4800e-173">示例</span><span class="sxs-lookup"><span data-stu-id="4800e-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4800e-174">请求</span><span class="sxs-lookup"><span data-stu-id="4800e-174">Request</span></span>

<span data-ttu-id="4800e-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4800e-175">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4800e-176">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4800e-176">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4800e-177">C#</span><span class="sxs-lookup"><span data-stu-id="4800e-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4800e-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4800e-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4800e-179">目标-C</span><span class="sxs-lookup"><span data-stu-id="4800e-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4800e-180">响应</span><span class="sxs-lookup"><span data-stu-id="4800e-180">Response</span></span>

<span data-ttu-id="4800e-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4800e-181">Here is an example of the response.</span></span>
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
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
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
