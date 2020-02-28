---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f440451ff18468c4f053eec11a62215cc551f654
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331288"
---
# <a name="update-subscription"></a><span data-ttu-id="a7745-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="a7745-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7745-104">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="a7745-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="a7745-105">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="a7745-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="a7745-106">为了避免丢失通知，应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="a7745-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="a7745-107">有关每种资源类型的最大订阅长度，请参阅[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="a7745-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7745-108">权限</span><span class="sxs-lookup"><span data-stu-id="a7745-108">Permissions</span></span>

<span data-ttu-id="a7745-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="a7745-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a7745-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7745-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7745-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="a7745-111">Supported resource</span></span> | <span data-ttu-id="a7745-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7745-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a7745-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7745-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7745-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7745-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="a7745-115">联系人</span><span class="sxs-lookup"><span data-stu-id="a7745-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a7745-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-116">Contacts.Read</span></span> | <span data-ttu-id="a7745-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-117">Contacts.Read</span></span> | <span data-ttu-id="a7745-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-118">Contacts.Read</span></span> |
|<span data-ttu-id="a7745-119">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="a7745-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a7745-120">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-120">Not supported</span></span> | <span data-ttu-id="a7745-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7745-121">Files.ReadWrite</span></span> | <span data-ttu-id="a7745-122">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-122">Not supported</span></span> |
|<span data-ttu-id="a7745-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="a7745-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a7745-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7745-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="a7745-125">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-125">Not supported</span></span> | <span data-ttu-id="a7745-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7745-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a7745-127">事件</span><span class="sxs-lookup"><span data-stu-id="a7745-127">event</span></span>](../resources/event.md) | <span data-ttu-id="a7745-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-128">Calendars.Read</span></span> | <span data-ttu-id="a7745-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-129">Calendars.Read</span></span> | <span data-ttu-id="a7745-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-130">Calendars.Read</span></span> |
|[<span data-ttu-id="a7745-131">组</span><span class="sxs-lookup"><span data-stu-id="a7745-131">group</span></span>](../resources/group.md) | <span data-ttu-id="a7745-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7745-132">Group.Read.All</span></span> | <span data-ttu-id="a7745-133">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-133">Not supported</span></span> | <span data-ttu-id="a7745-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7745-134">Group.Read.All</span></span> |
|[<span data-ttu-id="a7745-135">组对话</span><span class="sxs-lookup"><span data-stu-id="a7745-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a7745-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7745-136">Group.Read.All</span></span> | <span data-ttu-id="a7745-137">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-137">Not supported</span></span> | <span data-ttu-id="a7745-138">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-138">Not supported</span></span> |
|[<span data-ttu-id="a7745-139">list</span><span class="sxs-lookup"><span data-stu-id="a7745-139">list</span></span>](../resources/list.md) | <span data-ttu-id="a7745-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7745-140">Sites.ReadWrite.All</span></span> | <span data-ttu-id="a7745-141">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-141">Not supported</span></span> | <span data-ttu-id="a7745-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7745-142">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="a7745-143">邮件</span><span class="sxs-lookup"><span data-stu-id="a7745-143">message</span></span>](../resources/message.md) | <span data-ttu-id="a7745-144">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-144">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a7745-145">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a7745-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a7745-146">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="a7745-147">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="a7745-147">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="a7745-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7745-148">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a7745-149">不支持</span><span class="sxs-lookup"><span data-stu-id="a7745-149">Not supported</span></span> | <span data-ttu-id="a7745-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7745-150">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a7745-151">用户</span><span class="sxs-lookup"><span data-stu-id="a7745-151">user</span></span>](../resources/user.md) | <span data-ttu-id="a7745-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7745-152">User.Read.All</span></span> | <span data-ttu-id="a7745-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7745-153">User.Read.All</span></span> | <span data-ttu-id="a7745-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7745-154">User.Read.All</span></span> |

> <span data-ttu-id="a7745-155">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="a7745-155">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="a7745-156">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="a7745-156">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="a7745-157">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="a7745-157">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a7745-158">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="a7745-158">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a7745-159">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="a7745-159">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="a7745-160">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="a7745-160">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="a7745-161">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="a7745-161">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a7745-162">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="a7745-162">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a7745-163">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="a7745-163">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a7745-164">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="a7745-164">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a7745-165">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="a7745-165">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="a7745-166">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7745-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7745-167">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7745-167">Request headers</span></span>

| <span data-ttu-id="a7745-168">名称</span><span class="sxs-lookup"><span data-stu-id="a7745-168">Name</span></span>       | <span data-ttu-id="a7745-169">类型</span><span class="sxs-lookup"><span data-stu-id="a7745-169">Type</span></span> | <span data-ttu-id="a7745-170">说明</span><span class="sxs-lookup"><span data-stu-id="a7745-170">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7745-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7745-171">Authorization</span></span>  | <span data-ttu-id="a7745-172">string</span><span class="sxs-lookup"><span data-stu-id="a7745-172">string</span></span>  | <span data-ttu-id="a7745-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7745-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a7745-175">响应</span><span class="sxs-lookup"><span data-stu-id="a7745-175">Response</span></span>

<span data-ttu-id="a7745-176">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7745-176">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7745-177">示例</span><span class="sxs-lookup"><span data-stu-id="a7745-177">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a7745-178">请求</span><span class="sxs-lookup"><span data-stu-id="a7745-178">Request</span></span>

<span data-ttu-id="a7745-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7745-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7745-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7745-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a7745-181">C#</span><span class="sxs-lookup"><span data-stu-id="a7745-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7745-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7745-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7745-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7745-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a7745-184">响应</span><span class="sxs-lookup"><span data-stu-id="a7745-184">Response</span></span>

<span data-ttu-id="a7745-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a7745-185">Here is an example of the response.</span></span>
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
