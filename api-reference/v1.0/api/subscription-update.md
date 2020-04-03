---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d8a434c6760635fef602b77bbc6631d52c666f40
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108457"
---
# <a name="update-subscription"></a><span data-ttu-id="121a1-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="121a1-103">Update subscription</span></span>

<span data-ttu-id="121a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="121a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="121a1-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="121a1-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="121a1-106">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="121a1-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="121a1-107">为了避免丢失通知，应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="121a1-107">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="121a1-108">有关每种资源类型的最大订阅长度，请参阅[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="121a1-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="121a1-109">权限</span><span class="sxs-lookup"><span data-stu-id="121a1-109">Permissions</span></span>

<span data-ttu-id="121a1-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="121a1-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="121a1-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="121a1-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="121a1-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="121a1-112">Supported resource</span></span> | <span data-ttu-id="121a1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="121a1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="121a1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="121a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="121a1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="121a1-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="121a1-116">联系人</span><span class="sxs-lookup"><span data-stu-id="121a1-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="121a1-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-117">Contacts.Read</span></span> | <span data-ttu-id="121a1-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-118">Contacts.Read</span></span> | <span data-ttu-id="121a1-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-119">Contacts.Read</span></span> |
|<span data-ttu-id="121a1-120">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="121a1-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="121a1-121">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-121">Not supported</span></span> | <span data-ttu-id="121a1-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="121a1-122">Files.ReadWrite</span></span> | <span data-ttu-id="121a1-123">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-123">Not supported</span></span> |
|<span data-ttu-id="121a1-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="121a1-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="121a1-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121a1-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="121a1-126">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-126">Not supported</span></span> | <span data-ttu-id="121a1-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121a1-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="121a1-128">事件</span><span class="sxs-lookup"><span data-stu-id="121a1-128">event</span></span>](../resources/event.md) | <span data-ttu-id="121a1-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-129">Calendars.Read</span></span> | <span data-ttu-id="121a1-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-130">Calendars.Read</span></span> | <span data-ttu-id="121a1-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-131">Calendars.Read</span></span> |
|[<span data-ttu-id="121a1-132">组</span><span class="sxs-lookup"><span data-stu-id="121a1-132">group</span></span>](../resources/group.md) | <span data-ttu-id="121a1-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="121a1-133">Group.Read.All</span></span> | <span data-ttu-id="121a1-134">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-134">Not supported</span></span> | <span data-ttu-id="121a1-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="121a1-135">Group.Read.All</span></span> |
|[<span data-ttu-id="121a1-136">组对话</span><span class="sxs-lookup"><span data-stu-id="121a1-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="121a1-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="121a1-137">Group.Read.All</span></span> | <span data-ttu-id="121a1-138">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-138">Not supported</span></span> | <span data-ttu-id="121a1-139">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-139">Not supported</span></span> |
|[<span data-ttu-id="121a1-140">list</span><span class="sxs-lookup"><span data-stu-id="121a1-140">list</span></span>](../resources/list.md) | <span data-ttu-id="121a1-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121a1-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="121a1-142">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-142">Not supported</span></span> | <span data-ttu-id="121a1-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121a1-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="121a1-144">邮件</span><span class="sxs-lookup"><span data-stu-id="121a1-144">message</span></span>](../resources/message.md) | <span data-ttu-id="121a1-145">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="121a1-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="121a1-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="121a1-147">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="121a1-148">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="121a1-148">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="121a1-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121a1-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="121a1-150">不支持</span><span class="sxs-lookup"><span data-stu-id="121a1-150">Not supported</span></span> | <span data-ttu-id="121a1-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="121a1-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="121a1-152">用户</span><span class="sxs-lookup"><span data-stu-id="121a1-152">user</span></span>](../resources/user.md) | <span data-ttu-id="121a1-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="121a1-153">User.Read.All</span></span> | <span data-ttu-id="121a1-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="121a1-154">User.Read.All</span></span> | <span data-ttu-id="121a1-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="121a1-155">User.Read.All</span></span> |

> <span data-ttu-id="121a1-156">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="121a1-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="121a1-157">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="121a1-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="121a1-158">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="121a1-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="121a1-159">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="121a1-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="121a1-160">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="121a1-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="121a1-161">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="121a1-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="121a1-162">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="121a1-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="121a1-163">这意味着，您不能使用委派的权限日历。读取它可订阅其他用户的邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="121a1-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="121a1-164">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="121a1-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="121a1-165">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="121a1-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="121a1-166">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="121a1-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="121a1-167">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="121a1-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="121a1-168">请求标头</span><span class="sxs-lookup"><span data-stu-id="121a1-168">Request headers</span></span>

| <span data-ttu-id="121a1-169">名称</span><span class="sxs-lookup"><span data-stu-id="121a1-169">Name</span></span>       | <span data-ttu-id="121a1-170">类型</span><span class="sxs-lookup"><span data-stu-id="121a1-170">Type</span></span> | <span data-ttu-id="121a1-171">说明</span><span class="sxs-lookup"><span data-stu-id="121a1-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="121a1-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="121a1-172">Authorization</span></span>  | <span data-ttu-id="121a1-173">string</span><span class="sxs-lookup"><span data-stu-id="121a1-173">string</span></span>  | <span data-ttu-id="121a1-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="121a1-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="121a1-176">响应</span><span class="sxs-lookup"><span data-stu-id="121a1-176">Response</span></span>

<span data-ttu-id="121a1-177">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="121a1-177">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="121a1-178">示例</span><span class="sxs-lookup"><span data-stu-id="121a1-178">Example</span></span>

##### <a name="request"></a><span data-ttu-id="121a1-179">请求</span><span class="sxs-lookup"><span data-stu-id="121a1-179">Request</span></span>

<span data-ttu-id="121a1-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="121a1-180">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="121a1-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="121a1-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="121a1-182">C#</span><span class="sxs-lookup"><span data-stu-id="121a1-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="121a1-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="121a1-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="121a1-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="121a1-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="121a1-185">Java</span><span class="sxs-lookup"><span data-stu-id="121a1-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="121a1-186">响应</span><span class="sxs-lookup"><span data-stu-id="121a1-186">Response</span></span>

<span data-ttu-id="121a1-187">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="121a1-187">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
